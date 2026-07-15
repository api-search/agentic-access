---
acting_count: 283
action_class_counts:
  acting: 283
  connected: 153
api_specs:
- filename: prefect-openapi.json
  format: json
  label: Prefect Cloud REST API
  slug: prefect-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prefect/refs/heads/main/openapi/prefect-openapi.json
consequence_counts:
  physical: 35
  read: 153
  safety-critical: 6
  write: 242
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Prefect Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/accounts/{account_id}/invitations/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/concurrency_limits/tag/{tag}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/invitations/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/me/profile-image/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/me/sessions/{session_id}/terminate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/account_memberships/count
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/account_memberships/filter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/account_memberships/set_active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/accounts/{account_id}/account_memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/accounts/{account_id}/account_memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/accounts/{account_id}/account_memberships/{id}/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/bulk_delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/count
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/filter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/get_scheduled_flow_runs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/my-access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/paginate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}/access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}/branch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}/create_flow_run
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{account_id}/workspaces/{workspace_id}/deployments/{id}/create_flow_run/bulk
operation_count: 436
overview: 'Prefect exposes 436 API operations that an AI agent could call, of which 283 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 153 read, 242 write, 35 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prefect
provider_slug: prefect
slug: prefect-agentic-access
source_filename: prefect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/prefect-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 436\n  by_action_class:\n    connected: 153\n    acting: 283\n  by_consequence:\n    read: 153\n    write: 242\n    physical: 35\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /api/workspace_scopes\n  method: get\n  operationId: get_workspace_scopes_api_workspace_scopes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/permissions\n  method: get\n  operationId: list_permissions_api_accounts_permissions_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}\n  method: get\n  operationId: read_account_api_accounts__account_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}\n  method: patch\n  operationId: update_account_api_accounts__account_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}\n  method: delete\n  operationId: delete_account_api_accounts__account_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/settings\n  method: get\n  operationId: read_account_settings_api_accounts__account_id__settings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/settings\n  method: patch\n  operationId: update_account_settings_api_accounts__account_id__settings_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/domains\n  method: get\n  operationId: read_account_domains_api_accounts__account_id__domains_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/domains\n  method: patch\n  operationId: update_account_domains_api_accounts__account_id__domains_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/usage_limits\n  method: get\n  operationId: read_account_usage_limits_api_accounts__account_id__usage_limits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/usage\n  method: get\n  operationId: read_account_usage_api_accounts__account_id__usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/image\n  method: get\n  operationId: get_account_image_api_accounts__account_id__image_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/image\n  method: put\n  operationId: upload_account_image_api_accounts__account_id__image_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/image\n  method: delete\n  operationId: delete_account_image_api_accounts__account_id__image_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/\n  method: post\n  operationId: create_team_api_accounts__account_id__teams__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/{id}\n  method: get\n  operationId: read_team_api_accounts__account_id__teams__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/teams/{id}\n  method: put\n  operationId: update_team_api_accounts__account_id__teams__id__put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/{id}\n  method: delete\n  operationId: delete_team_api_accounts__account_id__teams__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/filter\n  method: post\n  operationId: read_teams_api_accounts__account_id__teams_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/{id}/members\n  method: put\n  operationId: upsert_team_members_api_accounts__account_id__teams__id__members_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/teams/{team_id}/members/{actor_id}\n  method: delete\n  operationId: remove_team_member_api_accounts__account_id__teams__team_id__members__actor_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/filter\n\
  \  method: post\n  operationId: read_account_memberships_api_accounts__account_id__account_memberships_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/count\n  method: post\n  operationId: count_account_memberships_api_accounts__account_id__account_memberships_count_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/by-user/{user_id}\n\
  \  method: get\n  operationId: read_account_membership_by_user_api_accounts__account_id__account_memberships_by_user__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/account_memberships/by-bot/{bot_id}\n  method: get\n  operationId: read_account_membership_by_bot_api_accounts__account_id__account_memberships_by_bot__bot_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/account_memberships/{id}\n  method: get\n  operationId: read_account_membership_api_accounts__account_id__account_memberships__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/account_memberships/{id}\n\
  \  method: patch\n  operationId: update_account_membership_api_accounts__account_id__account_memberships__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/{id}\n  method: delete\n  operationId: delete_account_membership_api_accounts__account_id__account_memberships__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/{id}/active\n\
  \  method: patch\n  operationId: toggle_account_membership_active_api_accounts__account_id__account_memberships__id__active_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_memberships/set_active\n  method: post\n  operationId: bulk_set_account_membership_active_api_accounts__account_id__account_memberships_set_active_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_roles/{id}\n\
  \  method: get\n  operationId: read_account_role_api_accounts__account_id__account_roles__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/account_roles/{id}\n  method: patch\n  operationId: update_account_role_api_accounts__account_id__account_roles__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_roles/{id}\n  method: delete\n  operationId: delete_account_role_api_accounts__account_id__account_roles__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/account_roles/filter\n  method: post\n  operationId: read_account_roles_api_accounts__account_id__account_roles_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/sso/setup_url\n  method: get\n  operationId: read_sso_setup_url_api_accounts__account_id__sso_setup_url_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/sso/dsync_setup_url\n  method: get\n  operationId: read_dsync_setup_url_api_accounts__account_id__sso_dsync_setup_url_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/sso/validate\n  method: post\n  operationId: validate_api_accounts__account_id__sso_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/sso/integrations\n  method: get\n  operationId: integrations_api_accounts__account_id__sso_integrations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/sso/integrations/{integration_id}\n  method: delete\n  operationId: remove_integration_api_accounts__account_id__sso_integrations__integration_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/\n  method: post\n  operationId: create_bot_api_accounts__account_id__bots__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/{id}\n  method: get\n  operationId: read_bot_api_accounts__account_id__bots__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/bots/{id}\n  method:\
  \ patch\n  operationId: update_bot_api_accounts__account_id__bots__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/{id}\n  method: delete\n  operationId: delete_bot_api_accounts__account_id__bots__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/filter\n  method: post\n  operationId: read_bots_api_accounts__account_id__bots_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/{id}/rotate_api_key\n  method: post\n  operationId: rotate_api_key_api_accounts__account_id__bots__id__rotate_api_key_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/bots/{id}/read_bot_api_keys\n  method: get\n  operationId: read_bot_api_keys_api_accounts__account_id__bots__id__read_bot_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/bots/{id}/delete_bot_api_key/{api_key_id}\n\
  \  method: delete\n  operationId: delete_bot_api_key_api_accounts__account_id__bots__id__delete_bot_api_key__api_key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/invitations/\n  method: post\n  operationId: create_invitation_api_accounts__account_id__invitations__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/invitations/{id}\n  method: get\n  operationId: read_invitation_api_accounts__account_id__invitations__id__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/invitations/filter\n  method: post\n  operationId: read_invitations_api_accounts__account_id__invitations_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/invitations/count\n  method: post\n  operationId: count_invitations_api_accounts__account_id__invitations_count_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/invitations/{id}/revoke\n\
  \  method: post\n  operationId: revoke_invitation_api_accounts__account_id__invitations__id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/\n  method: post\n  operationId: create_workspace_api_accounts__account_id__workspaces__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}\n  method: get\n  operationId: read_workspace_api_accounts__account_id__workspaces__workspace_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}\n  method: patch\n  operationId: update_workspace_api_accounts__account_id__workspaces__workspace_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}\n  method: delete\n  operationId: delete_workspace_api_accounts__account_id__workspaces__workspace_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/managed_execution/details\n  method: get\n  operationId: read_managed_execution_details_api_accounts__account_id__workspaces__workspace_id__managed_execution_details_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/filter\n  method: post\n  operationId: read_workspaces_api_accounts__account_id__workspaces_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/transfer\n  method: post\n  operationId: transfer_workspace_api_accounts__account_id__workspaces__workspace_id__transfer_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/validate_transfer\n  method: post\n  operationId: validate_transfer_workspace_api_accounts__account_id__workspaces__workspace_id__validate_transfer_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspaces/{workspace_id}\n  method: get\n  operationId: find_workspace_without_account_id_api_workspaces__workspace_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/settings\n  method: get\n  operationId: read_workspace_settings_api_accounts__account_id__workspaces__workspace_id__settings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/settings\n  method: patch\n  operationId: update_workspace_settings_api_accounts__account_id__workspaces__workspace_id__settings_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspace_roles/\n\
  \  method: post\n  operationId: create_workspace_role_api_accounts__account_id__workspace_roles__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspace_roles/{id}\n  method: patch\n  operationId: update_workspace_role_api_accounts__account_id__workspace_roles__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspace_roles/{id}\n  method: delete\n  operationId: delete_workspace_role_api_accounts__account_id__workspace_roles__id__delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspace_roles/{id}\n  method: get\n  operationId: read_workspace_role_api_accounts__account_id__workspace_roles__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspace_roles/filter\n  method: post\n  operationId: read_workspace_roles_api_accounts__account_id__workspace_roles_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/accounts/{account_id}/rate-limits/status\n  method: get\n  operationId: read_rate_limit_status_api_accounts__account_id__rate_limits_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/usage\n  method: get\n  operationId: read_rate_limit_usage_api_accounts__account_id__rate_limits_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/usage/download\n  method: get\n  operationId: download_rate_limit_usage_api_accounts__account_id__rate_limits_usage_download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/orchestration-api\n  method:\
  \ get\n  operationId: read_orchestration_api_grouped_usage_api_accounts__account_id__rate_limits_orchestration_api_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/events\n  method: get\n  operationId: read_events_grouped_usage_api_accounts__account_id__rate_limits_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/api-key-names\n  method: get\n  operationId: list_api_key_names_api_accounts__account_id__rate_limits_api_key_names_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limits/actor-names\n  method: get\n  operationId: list_actor_names_api_accounts__account_id__rate_limits_actor_names_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limit-allocations/\n  method: get\n  operationId: read_workspace_rate_limit_allocations_api_accounts__account_id__rate_limit_allocations__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/rate-limit-allocations/\n  method: put\n  operationId: upsert_workspace_rate_limit_allocations_api_accounts__account_id__rate_limit_allocations__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/invitations/\n\
  \  method: post\n  operationId: create_workspace_invitation_api_accounts__account_id__workspaces__workspace_id__invitations__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/invitations/{id}\n  method: get\n  operationId: read_workspace_invitation_api_accounts__account_id__workspaces__workspace_id__invitations__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/invitations/filter\n  method: post\n  operationId: read_workspace_invitations_api_accounts__account_id__workspaces__workspace_id__invitations_filter_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/invitations/{id}/revoke\n  method: post\n  operationId: revoke_workspace_invitation_api_accounts__account_id__workspaces__workspace_id__invitations__id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/user_access/\n  method: post\n  operationId: upsert_workspace_user_access_api_accounts__account_id__workspaces__workspace_id__user_access__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/user_access/filter\n  method: post\n  operationId: read_workspace_user_accesses_api_accounts__account_id__workspaces__workspace_id__user_access_filter_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/user_access/{id}\n  method: get\n  operationId: read_workspace_user_access_api_accounts__account_id__workspaces__workspace_id__user_access__id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/workspaces/{workspace_id}/user_access/{id}\n  method: delete\n  operationId: delete_workspace_user_access_api_accounts__account_id__workspaces__workspace_id__user_access__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      t\n\n# --- truncated at 32 KB (180 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/prefect/refs/heads/main/agentic-access/prefect-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prefect/refs/heads/main/agentic-access/prefect-agentic-access.yml
summary_line: 436 operations · 283 acting · 6 human-in-the-loop
tags:
- Automation
- Data Pipelines
- Orchestration
- Python
- Workflows
---
