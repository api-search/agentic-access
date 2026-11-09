---
acting_count: 49
action_class_counts:
  acting: 49
  connected: 47
api_specs:
- filename: bugbug-io-components-api-openapi.yml
  format: yaml
  label: BugBug Components API
  slug: bugbug-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-components-api-openapi.yml
- filename: bugbug-io-config-api-openapi.yml
  format: yaml
  label: BugBug Config API
  slug: bugbug-io-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-config-api-openapi.yml
- filename: bugbug-io-folders-api-openapi.yml
  format: yaml
  label: BugBug Folders API
  slug: bugbug-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-folders-api-openapi.yml
- filename: bugbug-io-groups-api-openapi.yml
  format: yaml
  label: BugBug Groups API
  slug: bugbug-io-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-groups-api-openapi.yml
- filename: bugbug-io-import-export-api-openapi.yml
  format: yaml
  label: BugBug Import / Export API
  slug: bugbug-io-import-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-import-export-api-openapi.yml
- filename: bugbug-io-organizations-api-openapi.yml
  format: yaml
  label: BugBug Organizations API
  slug: bugbug-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-organizations-api-openapi.yml
- filename: bugbug-io-profiles-api-openapi.yml
  format: yaml
  label: BugBug Profiles API
  slug: bugbug-io-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-profiles-api-openapi.yml
- filename: bugbug-io-projects-api-openapi.yml
  format: yaml
  label: BugBug Projects API
  slug: bugbug-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-projects-api-openapi.yml
- filename: bugbug-io-settings-api-openapi.yml
  format: yaml
  label: BugBug Settings API
  slug: bugbug-io-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-settings-api-openapi.yml
- filename: bugbug-io-step-runs-api-openapi.yml
  format: yaml
  label: BugBug Step runs API
  slug: bugbug-io-step-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-step-runs-api-openapi.yml
- filename: bugbug-io-steps-api-openapi.yml
  format: yaml
  label: BugBug Steps API
  slug: bugbug-io-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-steps-api-openapi.yml
- filename: bugbug-io-suite-runs-api-openapi.yml
  format: yaml
  label: BugBug Suite runs API
  slug: bugbug-io-suite-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suite-runs-api-openapi.yml
- filename: bugbug-io-suites-api-openapi.yml
  format: yaml
  label: BugBug Suites API
  slug: bugbug-io-suites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suites-api-openapi.yml
- filename: bugbug-io-tags-api-openapi.yml
  format: yaml
  label: BugBug Tags API
  slug: bugbug-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tags-api-openapi.yml
- filename: bugbug-io-test-runs-api-openapi.yml
  format: yaml
  label: BugBug Test runs API
  slug: bugbug-io-test-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-test-runs-api-openapi.yml
- filename: bugbug-io-tests-api-openapi.yml
  format: yaml
  label: BugBug Tests API
  slug: bugbug-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tests-api-openapi.yml
- filename: bugbug-io-variables-api-openapi.yml
  format: yaml
  label: BugBug Variables API
  slug: bugbug-io-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-variables-api-openapi.yml
- filename: bugbug-io-visual-regression-api-openapi.yml
  format: yaml
  label: BugBug Visual regression API
  slug: bugbug-io-visual-regression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-visual-regression-api-openapi.yml
consequence_counts:
  read: 47
  safety-critical: 2
  write: 47
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Bugbug Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/suiteruns/{id}/stop/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/testruns/{id}/stop/
operation_count: 96
overview: 'BugBug exposes 96 API operations that an AI agent could call, of which 49 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read, 47 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BugBug
provider_slug: bugbug-io
slug: bugbug-io-agentic-access
source_filename: bugbug-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/bugbug-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 96\n  by_action_class:\n    connected: 47\n    acting: 49\n  by_consequence:\n    read: 47\n    write: 47\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/components/\n  method: get\n  operationId: v2_components_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/components/\n  method: post\n  operationId: v2_components_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/components/{id}/usage/\n  method: get\n  operationId: v2_components_usage_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/config/ips/\n  method: get\n  operationId: v2_config_ips_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/config/status/\n  method: get\n  operationId: v2_config_status_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/folders/\n  method: get\n  operationId: v2_folders_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/folders/\n  method: post\n  operationId: v2_folders_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folders/{id}/\n  method: get\n  operationId: v2_folders_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/folders/{id}/\n  method: patch\n  operationId: v2_folders_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folders/{id}/\n\
  \  method: delete\n  operationId: v2_folders_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folders/tree/\n  method: get\n  operationId: v2_folders_tree_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/\n  method: get\n  operationId: v2_groups_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/\n  method: post\n  operationId: v2_groups_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/groups/{id}/\n  method: get\n  operationId: v2_groups_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/{id}/\n  method: put\n  operationId: v2_groups_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/groups/{id}/\n  method: patch\n  operationId: v2_groups_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/groups/{id}/\n  method: delete\n  operationId: v2_groups_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/\n  method: get\n  operationId: v2_organizations_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/profiles/\n  method: get\n  operationId: v2_profiles_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/profiles/{id}/\n  method: get\n  operationId: v2_profiles_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/project/export/\n  method: get\n  operationId: v2_project_export_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/project/import/check/\n  method: post\n  operationId: v2_project_import_check_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/project/import/run/\n  method: post\n  operationId: v2_project_import_run_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/project/import/validate/\n  method: post\n  operationId: v2_project_import_validate_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/\n  method: get\n  operationId: v2_projects_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project_pk}/backups/\n  method: get\n  operationId: v2_projects_backups_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project_pk}/backups/{id}/download/\n  method: get\n  operationId: v2_projects_backups_download_retrieve\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project_pk}/settings/\n  method: get\n  operationId: v2_projects_settings_list_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/settings/\n  method: get\n  operationId: v2_projects_settings_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/schema/yaml/v1/\n  method: get\n  operationId: v2_schema_yaml_v1_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/settings/\n  method: get\n  operationId: v2_settings_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stepruns/{id}/\n  method: get\n  operationId: v2_stepruns_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/steps/\n  method: post\n  operationId: v2_steps_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/steps/{id}/\n  method: get\n  operationId: v2_steps_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/steps/{id}/\n  method: put\n  operationId: v2_steps_update\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/steps/{id}/\n  method: patch\n  operationId: v2_steps_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/steps/{id}/\n  method: delete\n  operationId: v2_steps_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suiteruns/\n  method: get\n  operationId: v2_suiteruns_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/\n  method: post\n  operationId: v2_suiteruns_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suiteruns/{id}/\n  method: get\n  operationId: v2_suiteruns_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/{id}/\n  method: patch\n  operationId: v2_suiteruns_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suiteruns/{id}/debug-artifacts/\n  method: get\n  operationId: v2_suiteruns_debug_artifacts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/{id}/report/junit/\n  method: get\n  operationId: v2_suiteruns_report_junit_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/{id}/screenshots/\n  method: get\n  operationId: v2_suiteruns_screenshots_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/{id}/status/\n  method: get\n  operationId: v2_suiteruns_status_retrieve\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suiteruns/{id}/stop/\n  method: post\n  operationId: v2_suiteruns_stop_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/suiteruns/{id}/tags/\n  method: put\n  operationId: v2_suiteruns_tags_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suites/\n  method: get\n  operationId: v2_suites_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suites/\n  method: post\n  operationId: v2_suites_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suites/{id}/\n  method: get\n  operationId: v2_suites_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/suites/{id}/\n  method: put\n  operationId: v2_suites_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/suites/{id}/\n  method: patch\n  operationId: v2_suites_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suites/{id}/\n  method: delete\n  operationId: v2_suites_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/suites/{id}/tags/\n  method: put\n  operationId: v2_suites_tags_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tags/\n  method: get\n  operationId: v2_tags_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tags/\n  method: post\n  operationId: v2_tags_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tags/{id}/\n  method: get\n  operationId: v2_tags_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tags/{id}/\n  method: patch\n  operationId: v2_tags_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tags/{id}/\n  method: delete\n  operationId: v2_tags_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/testruns/\n  method: get\n  operationId: v2_testruns_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/\n  method: post\n  operationId: v2_testruns_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/testruns/{id}/\n  method: get\n  operationId: v2_testruns_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/\n  method: patch\n  operationId: v2_testruns_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/testruns/{id}/debug-artifacts/\n  method: get\n  operationId: v2_testruns_debug_artifacts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/debug-artifacts/{artifact_type}/\n\
  \  method: get\n  operationId: v2_testruns_debug_artifacts_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/logs/\n  method: get\n  operationId: v2_testruns_logs_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/report/junit/\n  method: get\n  operationId: v2_testruns_report_junit_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/screenshots/\n  method: get\n  operationId: v2_testruns_screenshots_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/status/\n  method: get\n\
  \  operationId: v2_testruns_status_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/testruns/{id}/stop/\n  method: post\n  operationId: v2_testruns_stop_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/testruns/{id}/tags/\n  method: put\n  operationId: v2_testruns_tags_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/\n  method: get\n  operationId:\
  \ v2_tests_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tests/\n  method: post\n  operationId: v2_tests_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/\n  method: get\n  operationId: v2_tests_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tests/{id}/\n  method: put\n  operationId: v2_tests_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/\n  method: patch\n  operationId: v2_tests_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/\n  method: delete\n  operationId: v2_tests_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/export/{fmt}/\n  method: get\n  operationId: v2_tests_export_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/tests/{id}/insert-component/\n  method: post\n  operationId: v2_tests_insert_component_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/tags/\n  method: put\n  operationId: v2_tests_tags_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/unlink-component/\n  method: post\n  operationId: v2_tests_unlink_component_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/update-group-position/\n  method: post\n  operationId: v2_tests_update_group_position_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/{id}/update-step-position/\n  method: post\n  operationId: v2_tests_update_step_position_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/import/\n  method: post\n  operationId: v2_tests_import_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tests/import/check/\n  method: post\n  operationId: v2_tests_import_check_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/variables/\n  method: get\n  operationId: v2_variables_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/variables/\n  method: post\n  operationId: v2_variables_create\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/variables/{key}/\n  method: get\n  operationId: v2_variables_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/variables/{key}/\n  method: patch\n  operationId: v2_variables_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/visual-regression/reference-screenshots/\n  method: get\n  operationId: v2_visual_regression_reference_screenshots_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/visual-regression/reference-screenshots/\n  method: post\n  operationId: v2_visual_regression_reference_screenshots_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/visual-regression/reference-screenshots/{id}/\n  method: get\n  operationId: v2_visual_regression_reference_screenshots_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/visual-regression/reference-screenshots/{id}/\n  method: put\n  operationId: v2_visual_regression_reference_screenshots_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/visual-regression/reference-screenshots/{id}/\n  method: patch\n  operationId: v2_visual_regression_reference_screenshots_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/visual-regression/reference-screenshots/{id}/\n  method: delete\n  operationId: v2_visual_regression_reference_screenshots_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/visual-regression/resolve/\n  method: post\n  operationId: v2_visual_regression_resolve_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bugbug-io/agentic-access/bugbug-io-agentic-access.yml
summary_line: 96 operations · 49 acting · 2 human-in-the-loop
tags:
- Company
- Testing
- Automation
- Software-as-a-Service
- Low-Code
- No-Code
---
