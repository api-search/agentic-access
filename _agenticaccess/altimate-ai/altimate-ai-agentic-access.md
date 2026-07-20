---
acting_count: 396
action_class_counts:
  acting: 396
  connected: 608
api_specs:
- filename: altimate-ai-openapi-original.json
  format: json
  label: Altimate AI Platform API
  slug: altimate-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/openapi/altimate-ai-openapi-original.json
consequence_counts:
  physical: 23
  read: 608
  safety-critical: 4
  write: 369
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Altimate Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /preset/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /preset/{preset_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /preset/{preset_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workflow/dashboard/commands
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workflow/dashboard/sessions/{session_id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /external/stripe/webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/ownership-rules/conflicting-team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/ownership-rules/conflicting-team/download
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/ownership-rules/cost-preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/{user_group_id}/ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /groups/{user_group_id}/ownership/{ownership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notification/send/slack
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notification/send_datamate_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/checkout/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/downgrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/downgrade/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/downgrade/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/enterprise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/enterprise/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/wallet/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/wallet/deposit/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment/wallet/settings
operation_count: 1004
overview: 'Altimate AI exposes 1004 API operations that an AI agent could call, of which 396 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 608 read, 369 write, 23 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Altimate AI
provider_slug: altimate-ai
slug: altimate-ai-agentic-access
source_filename: altimate-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/altimate-ai-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1004\n  by_action_class:\n    acting: 396\n    connected: 608\n  by_consequence:\n    write: 369\n    read: 608\n    safety-critical: 4\n    physical: 23\n  human_in_the_loop_required: 4\noperations:\n- path: /auth/login\n  method: post\n  operationId: auth_login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/supertokens_user_info\n  method: get\n\
  \  operationId: supertokens_user_info_auth_supertokens_user_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/register-sso\n  method: post\n  operationId: register_new_user_sso_auth_register_sso_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/company-info\n  method: get\n  operationId: company_info_auth_company_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/group-tenants\n  method: post\n  operationId: group_tenants_auth_group_tenants_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/register-invite\n  method: post\n  operationId: register_invite_auth_register_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/connections\n  method: get\n  operationId: connections_auth_connections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/forgot-password\n  method: post\n  operationId: forgot_password_auth_forgot_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/reset-password\n  method: post\n  operationId: reset_password_auth_reset_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/tenant-info\n  method: get\n  operationId: tenant_info_auth_tenant_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/tenant-info\n  method: patch\n  operationId: patch_tenant_info_auth_tenant_info_patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/regenerate_token\n  method: post\n  operationId: regenerate_token_auth_regenerate_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/clickhouse-rbac\n  method: get\n  operationId: get_clickhouse_rbac_api_clickhouse_rbac_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user-group-rules-stats\n  method: get\n  operationId: get_user_group_rules_stats_api_user_group_rules_stats_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user-group-rules-stats/tenants\n  method: get\n  operationId: get_tenants_api_user_group_rules_stats_tenants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /impersonate\n  method: post\n  operationId: impersonate_impersonate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /demo/create-demo-session\n  method: post\n  operationId: create_demo_session_demo_create_demo_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /demo/authenticate\n  method: post\n  operationId: authenticate_demo_session_demo_authenticate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/\n  method: get\n  operationId: user_get_all_users__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/download\n  method: get\n  operationId: user_download_all_users_download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /users/profile\n  method: patch\n  operationId: user_tz_edit_users_profile_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me\n  method: get\n  operationId: get_me_users_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/chat\n  method: get\n  operationId: user_get_all_users_chat_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/invite\n  method: post\n  operationId: invite_user_users_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/onboard\n  method: post\n  operationId: user_onboard_users_onboard_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/get_role\n  method: get\n  operationId: get_role_users_get_role_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/role_edit\n  method: post\n  operationId: user_role_edit_users_role_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/resolve_role_conflict\n  method: post\n  operationId: resolve_role_conflict_users_resolve_role_conflict_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/default_user_group\n  method: post\n  operationId: update_default_user_group_users_default_user_group_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}\n  method: get\n  operationId:\
  \ user_get_one_users__user_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}\n  method: patch\n  operationId: user_edit_users__user_uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}\n  method: delete\n  operationId: user_delete_users__user_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /permissions/\n  method: get\n  operationId: role_get_all_permissions__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions/\n  method: post\n  operationId: role_add_permissions__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /permissions/all\n  method: get\n  operationId: permissions_get_all_permissions_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions/{role_uuid}\n  method: get\n  operationId: role_get_one_permissions__role_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /permissions/{role_uuid}\n  method: patch\n  operationId: role_edit_permissions__role_uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /permissions/{role_uuid}\n  method: delete\n  operationId: role_delete_permissions__role_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/\n  method: get\n  operationId: group_get_all_groups__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /groups/\n  method: post\n  operationId: group_add_groups__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/get_all\n  method: get\n  operationId: group_get_all_unpaginated_groups_get_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}\n  method: get\n  operationId: group_get_one_groups__group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}\n  method: patch\n  operationId: group_edit_groups__group_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}\n  method: delete\n  operationId: group_delete_groups__group_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/rules/{rule_id}\n  method: delete\n  operationId: group_rule_delete_groups__group_id__rules__rule_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /groups/group_rule_file\n  method: post\n  operationId: upload_file_groups_group_rule_file_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/user_group_file\n  method: post\n  operationId: upload_file_groups_user_group_file_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/group_rules/{group_uuid}\n  method: get\n  operationId: upload_file_groups_group_rules__group_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /groups/{group_id}/users/{user_id}\n  method: delete\n  operationId: group_user_remove_groups__group_id__users__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/group_create\n  method: post\n  operationId: group_create_groups_group_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{user_group_id}/rules\n  method: post\n  operationId: add_group_rule_groups__user_group_id__rules_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{user_group_id}/members\n  method: post\n  operationId: add_group_member_groups__user_group_id__members_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{user_group_id}/ownership\n  method: post\n  operationId: add_group_ownership_groups__user_group_id__ownership_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{user_group_id}/ownership\n  method: get\n  operationId: get_group_ownership_groups__user_group_id__ownership_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{user_group_id}/ownership/{ownership_id}\n  method: delete\n  operationId: delete_group_ownership_groups__user_group_id__ownership__ownership_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/ownership-rules/cost-preview\n  method: post\n  operationId: get_ownership_cost_preview_groups_ownership_rules_cost_preview_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/ownership-rules/conflicting-team\n  method: post\n  operationId: get_conflicting_team_groups_ownership_rules_conflicting_team_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/ownership-rules/conflicting-team/download\n  method: post\n  operationId: download_conflicting_team_groups_ownership_rules_conflicting_team_download_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/ownership-rules/conflicts/{user_group_id}\n  method: get\n  operationId: get_ownership_conflicts_summary_groups_ownership_rules_conflicts__user_group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/ownership-rules/conflicts/{user_group_id}/details\n  method: get\n  operationId: get_ownership_conflict_details_groups_ownership_rules_conflicts__user_group_id__details_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/ownership-rules/conflicts/{user_group_id}/details/download\n\
  \  method: get\n  operationId: download_ownership_conflict_details_groups_ownership_rules_conflicts__user_group_id__details_download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso-group-mappings/targets\n  method: get\n  operationId: list_targets_sso_group_mappings_targets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso-group-mappings/config\n  method: get\n  operationId: get_config_sso_group_mappings_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso-group-mappings/config\n  method: put\n  operationId: update_config_sso_group_mappings_config_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/mappings\n  method: get\n  operationId: list_mappings_sso_group_mappings_mappings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso-group-mappings/mappings\n  method: post\n  operationId: create_mapping_sso_group_mappings_mappings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/mappings/{mapping_id}\n  method: put\n  operationId: update_mapping_sso_group_mappings_mappings__mapping_id__put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/mappings/{mapping_id}\n  method: delete\n  operationId: delete_mapping_sso_group_mappings_mappings__mapping_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/preview\n  method: post\n  operationId: preview_mappings_sso_group_mappings_preview_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/external-groups\n  method: get\n  operationId: list_external_groups_sso_group_mappings_external_groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sso-group-mappings/external-groups/upload\n  method: post\n  operationId: upload_external_groups_sso_group_mappings_external_groups_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/mappings/upload\n  method: post\n  operationId: upload_mappings_sso_group_mappings_mappings_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sso-group-mappings/audit-events\n  method: get\n  operationId: list_audit_events_sso_group_mappings_audit_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/team_rule_file\n  method: post\n  operationId: upload_team_rule_file_teams_team_rule_file_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/user_team_file\n  method: post\n  operationId: upload_user_team_file_teams_user_team_file_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/cost/graph\n  method: get\n  operationId: get_cost_teams_cost_graph_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/cost/period-comparison\n  method: get\n  operationId: get_cost_period_comparison_teams_cost_period_comparison_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/filters\n  method: get\n  operationId: get_filters_teams_filters_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/\n\
  \  method: get\n  operationId: company_get_all_companies__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/\n  method: post\n  operationId: company_add_companies__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_uuid}\n  method: get\n  operationId: company_get_one_companies__company_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_uuid}\n  method: patch\n  operationId: company_edit_companies__company_uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_uuid}\n  method: delete\n  operationId: company_delete_companies__company_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/available/{company}\n  method: get\n  operationId: company_available_companies_available__company__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/register\n  method: post\n  operationId: company_register_companies_register_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/verify-user\n  method: post\n  operationId: company_verify_user_companies_verify_user_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/get-all-companies/{email}\n  method: get\n  operationId: get_all_companies_by_email_companies_get_all_companies__email__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referral-codes\n  method: get\n  operationId: list_codes_referral_codes_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referral-codes\n  method: post\n  operationId: create_code_referral_codes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/\n  method: post\n  operationId: create_contract_in_registry_registries__registry_id__contracts__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/\n  method: get\n \
  \ operationId: get_contracts_by_registry_registries__registry_id__contracts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registries/{registry_id}/contracts/definitions/validate\n  method: post\n  operationId: validate_contract_definition_dry_run_registries__registry_id__contracts_definitions_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/{contract_id}\n  method: get\n  operationId: get_contracts_by_registry_and_id_registries__registry_id__contracts__contract_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /registries/{registry_id}/contracts/{contract_id}\n  method: delete\n  operationId: delete_contract_from_registry_by_id_registries__registry_id__contracts__contract_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/{contract_id}/validate\n  method: post\n  operationId: validate_registries__registry_id__contracts__contract_id__validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/{contract_id}/schedule_validation\n\
  \  method: post\n  operationId: schedule_validation_registries__registry_id__contracts__contract_id__schedule_validation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registries/{registry_id}/contracts/{contract_id}/configurations\n  method: get\n  operationId: get_contract_configuration_for_profile_registries__registry_id__contracts__contract_id__configurations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registries/\n  method: get\n  operationId: get_registry_registries__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r\n\
  \n# --- truncated at 32 KB (311 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/agentic-access/altimate-ai-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/agentic-access/altimate-ai-agentic-access.yml
summary_line: 1004 operations · 396 acting · 4 human-in-the-loop
tags:
- Company
- Data
- Data Engineering
- Artificial Intelligence
- Agents
- MCP
- dbt
- Data Governance
- Data Contracts
- Analytics Engineering
---
