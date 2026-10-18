---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 25
api_specs:
- filename: centaur-labs-add-and-manage-labels-api-openapi.yml
  format: yaml
  label: Centaur Labs Add and Manage Labels API
  slug: centaur-labs-add-and-manage-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-add-and-manage-labels-api-openapi.yml
- filename: centaur-labs-add-and-manage-projects-api-openapi.yml
  format: yaml
  label: Centaur Labs Add and Manage Projects API
  slug: centaur-labs-add-and-manage-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-add-and-manage-projects-api-openapi.yml
- filename: centaur-labs-add-and-manage-tasks-api-openapi.yml
  format: yaml
  label: Centaur Labs Add and Manage Tasks API
  slug: centaur-labs-add-and-manage-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-add-and-manage-tasks-api-openapi.yml
- filename: centaur-labs-create-and-manage-cases-api-openapi.yml
  format: yaml
  label: Centaur Labs Create and Manage Cases API
  slug: centaur-labs-create-and-manage-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-create-and-manage-cases-api-openapi.yml
- filename: centaur-labs-get-api-version-api-openapi.yml
  format: yaml
  label: Centaur Labs Get API Version API
  slug: centaur-labs-get-api-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-get-api-version-api-openapi.yml
- filename: centaur-labs-get-case-results-api-openapi.yml
  format: yaml
  label: Centaur Labs Get Case Results API
  slug: centaur-labs-get-case-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-get-case-results-api-openapi.yml
- filename: centaur-labs-get-task-results-api-openapi.yml
  format: yaml
  label: Centaur Labs Get Task Results API
  slug: centaur-labs-get-task-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-get-task-results-api-openapi.yml
- filename: centaur-labs-import-and-manage-data-api-openapi.yml
  format: yaml
  label: Centaur Labs Import and Manage Data API
  slug: centaur-labs-import-and-manage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-import-and-manage-data-api-openapi.yml
- filename: centaur-labs-login-api-openapi.yml
  format: yaml
  label: Centaur Labs Login API
  slug: centaur-labs-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-login-api-openapi.yml
- filename: centaur-labs-logout-api-openapi.yml
  format: yaml
  label: Centaur Labs Logout API
  slug: centaur-labs-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-logout-api-openapi.yml
- filename: centaur-labs-masks-public-api-openapi.yml
  format: yaml
  label: Centaur Labs Masks Public API
  slug: centaur-labs-masks-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-masks-public-api-openapi.yml
- filename: centaur-labs-reads-opinions-lookup-api-openapi.yml
  format: yaml
  label: Centaur Labs Reads (Opinions) Lookup API
  slug: centaur-labs-reads-opinions-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-reads-opinions-lookup-api-openapi.yml
- filename: centaur-labs-refresh-token-api-openapi.yml
  format: yaml
  label: Centaur Labs Refresh Token API
  slug: centaur-labs-refresh-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-refresh-token-api-openapi.yml
- filename: centaur-labs-tags-api-openapi.yml
  format: yaml
  label: Centaur Labs Tags API
  slug: centaur-labs-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-tags-api-openapi.yml
- filename: centaur-labs-test-token-api-openapi.yml
  format: yaml
  label: Centaur Labs Test Token API
  slug: centaur-labs-test-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-test-token-api-openapi.yml
- filename: centaur-labs-version-api-openapi.yml
  format: yaml
  label: Centaur Labs Version API
  slug: centaur-labs-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/openapi/centaur-labs-version-api-openapi.yml
consequence_counts:
  physical: 2
  read: 25
  safety-critical: 3
  write: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Centaur Labs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /assets/public/v1/add
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /cases/goldStandards/public/v1/set
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /cases/prelabels/public/v1/set
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /labelClasses/public/v1/groups/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /labelClasses/public/v1/reorder
operation_count: 76
overview: 'Centaur Labs exposes 76 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 46 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Centaur Labs
provider_slug: centaur-labs
slug: centaur-labs-agentic-access
source_filename: centaur-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/centaur-labs-authorization-api-openapi.yml, openapi/centaur-labs-ingest-api-openapi.yml,\n  openapi/centaur-labs-label-apis-openapi.yml, openapi/centaur-labs-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    acting: 51\n    connected: 25\n  by_consequence:\n    write: 46\n    read: 25\n    safety-critical: 3\n    physical: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /auth/public/v1/login\n  method: post\n  operationId: login_auth_public_v1_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/public/v1/logout\n  method: post\n  operationId: logout_auth_public_v1_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/public/v1/refreshToken\n  method: post\n  operationId: refresh_token_auth_public_v1_refreshToken_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/public/v1/testToken\n  method: post\n  operationId: test_token_auth_public_v1_testToken_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/public/v1/version\n  method: get\n  operationId: version_auth_public_v1_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /answers/public/v1/add\n  method: post\n  operationId: handler_add_answer_legacy_answers_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /answers/public/v1/delete\n  method: delete\n  operationId: handler_delete_answer_legacy_answers_public_v1_delete_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /answers/public/v1/update\n  method: patch\n  operationId: update_label_classes_answers_public_v1_update_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/public/v1/add\n  method: post\n  operationId: shared_add_asset_override_assets_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n \
  \     proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assets/public/v1/get\n  method: get\n  operationId: shared_get_asset_assets_public_v1_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/public/v1/list\n  method: get\n  operationId: public_list_assets_assets_public_v1_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/public/v1/listSeries\n  method: post\n  operationId: shared_list_series_assets_public_v1_listSeries_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /assets/public/v2/list\n  method: post\n  operationId: shared_list_assets_v2_assets_public_v2_list_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/custom/v1/update\n  method: patch\n  operationId: update_problem_cases_custom_v1_update_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/goldStandards/public/v1/set\n  method: patch\n  operationId: set_gold_standards_override_cases_goldStandards_public_v1_set_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cases/goldStandards/public/v1/unset\n  method: delete\n  operationId: unset_gs_from_problems_cases_goldStandards_public_v1_unset_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/prelabels/public/v1/set\n  method: put\n  operationId: handler_set_prelabels_override_cases_prelabels_public_v1_set_put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cases/prelabels/public/v1/unset\n  method: delete\n  operationId: handler_unset_prelabels_from_problems_cases_prelabels_public_v1_unset_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/public/v1/addImageFromFile\n  method: post\n  operationId: add_asset_and_case_from_file_cases_public_v1_addImageFromFile_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/public/v1/delete\n  method: delete\n\
  \  operationId: delete_case_cases_public_v1_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/public/v1/duplicate\n  method: post\n  operationId: handler_duplicate_case_cases_public_v1_duplicate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/public/api/v1/version\n  method: get\n  operationId: get_version_imports_public_api_v1_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /imports/public/v1/add\n  method: post\n  operationId: add_import_imports_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/public/v1/addAssetsFromURLs\n  method: post\n  operationId: add_assets_from_urls_imports_public_v1_addAssetsFromURLs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/public/v1/delete\n  method: delete\n  operationId: import_delete_imports_public_v1_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/public/v1/get\n  method: get\n  operationId: get_import_public_imports_public_v1_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/public/v1/list\n  method: get\n  operationId: list_import_imports_public_v1_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/public/v1/policy/get\n  method: get\n  operationId: get_import_policy_imports_public_v1_policy_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/public/v1/validateAccess\n  method:\
  \ get\n  operationId: validate_access_imports_public_v1_validateAccess_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labelClasses/public/v1/add\n  method: post\n  operationId: handler_add_answer_labelClasses_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/delete\n  method: delete\n  operationId: handler_delete_answer_labelClasses_public_v1_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /labelClasses/public/v1/groups\n  method: post\n  operationId: handler_add_label_class_group_labelClasses_public_v1_groups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/groups\n  method: get\n  operationId: handler_list_label_class_groups_labelClasses_public_v1_groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labelClasses/public/v1/groups/reorder\n  method: put\n  operationId: handler_reorder_label_class_groups_labelClasses_public_v1_groups_reorder_put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/groups/{label_class_group_id}\n  method: delete\n  operationId: handler_delete_label_class_group_labelClasses_public_v1_groups__label_class_group_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/groups/{label_class_group_id}\n  method: patch\n  operationId: handler_update_label_class_group_labelClasses_public_v1_groups__label_class_group_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/groups/{label_class_group_id}\n  method: get\n  operationId: handler_get_label_class_group_labelClasses_public_v1_groups__label_class_group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labelClasses/public/v1/groups/{label_class_group_id}/answers\n  method: post\n  operationId: handler_add_existing_answers_to_label_class_group_labelClasses_public_v1_groups__label_class_group_id__answers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/groups/{label_class_group_id}/answers\n\
  \  method: delete\n  operationId: handler_delete_answers_from_label_class_group_labelClasses_public_v1_groups__label_class_group_id__answers_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/reorder\n  method: put\n  operationId: handler_reorder_answers_labelClasses_public_v1_reorder_put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labelClasses/public/v1/update\n  method: patch\n  operationId: update_label_classes_labelClasses_public_v1_update_patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests/public/v1/add\n  method: post\n  operationId: add_files_manifest_manifests_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests/public/v1/get\n  method: get\n  operationId: get_manifest_manifests_public_v1_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/public/v1/add\n  method: post\n  operationId: create_project_public_projects_public_v1_add_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/public/v1/delete\n  method: delete\n  operationId: delete_project_projects_public_v1_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/public/v1/get\n  method: get\n  operationId: get_project_projects_public_v1_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/public/v1/list\n  method: get\n  operationId: list_projects_projects_public_v1_list_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/public/v1/set\n  method: patch\n  operationId: update_project_public_projects_public_v1_set_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/public/v1/add\n  method: post\n  operationId: public_add_tag_tags_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/public/v1/asset/add\n  method: post\n  operationId: public_add_asset_tag_tags_public_v1_asset_add_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/public/v1/asset/delete\n  method: delete\n  operationId: public_remove_asset_tag_tags_public_v1_asset_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/public/v1/asset/list\n  method: get\n  operationId: public_list_asset_tags_tags_public_v1_asset_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/public/v1/delete\n  method: delete\n\
  \  operationId: public_remove_tag_tags_public_v1_delete_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/public/v1/list\n  method: get\n  operationId: public_list_tags_tags_public_v1_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/assets/public/v1/add\n  method: post\n  operationId: add_asset_to_task_tasks_assets_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/goldStandards/public/v1/unset\n\
  \  method: delete\n  operationId: unset_gs_from_task_tasks_goldStandards_public_v1_unset_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/imports/public/v1/add\n  method: post\n  operationId: add_imports_to_task_public_tasks_imports_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/prelabels/public/v1/unset\n  method: delete\n  operationId: handler_unset_prelabels_from_task_tasks_prelabels_public_v1_unset_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/public/v1/add\n  method: post\n  operationId: task_add_public_tasks_public_v1_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/public/v1/duplicate\n  method: post\n  operationId: task_duplicate_tasks_public_v1_duplicate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/public/v1/get\n\
  \  method: get\n  operationId: task_get_tasks_public_v1_get_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/public/v1/instructions\n  method: post\n  operationId: task_set_instructions_tasks_public_v1_instructions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/public/v1/list\n  method: get\n  operationId: task_list_tasks_public_v1_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/public/v1/set\n  method: patch\n  operationId: task_update_public_tasks_public_v1_set_patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/public/v2/add\n  method: post\n  operationId: task_add_public_tasks_public_v2_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reads/public/v1/lookup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reads/public/v1/version\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v1/get\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v1/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v1/version\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v2/get\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v2/getResultsArchiveUrl\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v2/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/public/v2/version\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /masks/public/v1/commit\n  method: post\n  operationId: public_commit_masks_route_masks_public_v1_commit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /masks/public/v1/generate-presigned-urls\n  method: post\n  operationId: public_generate_presigned_urls_route_masks_public_v1_generate_presigned_urls_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/agentic-access/centaur-labs-agentic-access.yml
summary_line: 76 operations · 51 acting · 3 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Data Annotation
- Data Labeling
- Machine Learning
- Healthcare
- Medical Imaging
- Training Data
---
