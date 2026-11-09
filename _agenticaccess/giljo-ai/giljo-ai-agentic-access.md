---
acting_count: 42
action_class_counts:
  acting: 42
  connected: 34
api_specs:
- filename: giljo-ai-account-deletion-api-openapi.yml
  format: yaml
  label: giljo-ai Account Deletion API
  slug: giljo-ai-account-deletion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-account-deletion-api-openapi.yml
- filename: giljo-ai-account-lifecycle-api-openapi.yml
  format: yaml
  label: giljo-ai Account Lifecycle API
  slug: giljo-ai-account-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-account-lifecycle-api-openapi.yml
- filename: giljo-ai-auth-api-openapi.yml
  format: yaml
  label: giljo-ai Auth API
  slug: giljo-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-auth-api-openapi.yml
- filename: giljo-ai-comm-threads-api-openapi.yml
  format: yaml
  label: giljo-ai Comm Threads API
  slug: giljo-ai-comm-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-comm-threads-api-openapi.yml
- filename: giljo-ai-connected-accounts-api-openapi.yml
  format: yaml
  label: giljo-ai Connected Accounts API
  slug: giljo-ai-connected-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-connected-accounts-api-openapi.yml
- filename: giljo-ai-health-api-openapi.yml
  format: yaml
  label: giljo-ai Health API
  slug: giljo-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-health-api-openapi.yml
- filename: giljo-ai-legal-api-openapi.yml
  format: yaml
  label: giljo-ai Legal API
  slug: giljo-ai-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-legal-api-openapi.yml
- filename: giljo-ai-oauth-api-openapi.yml
  format: yaml
  label: giljo-ai OAuth API
  slug: giljo-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-oauth-api-openapi.yml
- filename: giljo-ai-oauth-dcr-api-openapi.yml
  format: yaml
  label: giljo-ai OAUTH Dcr API
  slug: giljo-ai-oauth-dcr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-oauth-dcr-api-openapi.yml
- filename: giljo-ai-social-login-api-openapi.yml
  format: yaml
  label: giljo-ai Social Login API
  slug: giljo-ai-social-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-social-login-api-openapi.yml
- filename: giljo-ai-task-statuses-api-openapi.yml
  format: yaml
  label: giljo-ai Task Statuses API
  slug: giljo-ai-task-statuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-task-statuses-api-openapi.yml
- filename: giljo-ai-tasks-api-openapi.yml
  format: yaml
  label: giljo-ai Tasks API
  slug: giljo-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-tasks-api-openapi.yml
- filename: giljo-ai-users-api-openapi.yml
  format: yaml
  label: giljo-ai Users API
  slug: giljo-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-users-api-openapi.yml
consequence_counts:
  read: 34
  safety-critical: 4
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Giljo Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/auth/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/saas/password-reset/confirm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/saas/password-reset/request
operation_count: 76
overview: 'giljo-ai exposes 76 API operations that an AI agent could call, of which 42 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 38 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: giljo-ai
provider_slug: giljo-ai
slug: giljo-ai-agentic-access
source_filename: giljo-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/amh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 34\n    acting: 42\n  by_consequence:\n    read: 34\n    write: 38\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/threads\n  method: get\n  operationId: list_threads_api_v1_threads_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads\n  method: post\n  operationId: create_thread_api_v1_threads_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/my-turn\n  method: get\n  operationId: get_my_turn_api_v1_threads_my_turn_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/attention\n  method: get\n  operationId: get_current_user_attention_api_v1_threads_attention_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/search\n  method: get\n  operationId: search_threads_api_v1_threads_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/deleted\n  method: get\n  operationId: list_deleted_threads_api_v1_threads_deleted_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/count\n  method: get\n  operationId: get_thread_count_api_v1_threads_count_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/{thread_id}\n  method: get\n  operationId: get_thread_history_api_v1_threads__thread_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/{thread_id}\n  method: patch\n  operationId: update_thread_api_v1_threads__thread_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/{thread_id}\n  method: delete\n  operationId: delete_thread_api_v1_threads__thread_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/{thread_id}/participants\n  method: get\n  operationId: get_participants_api_v1_threads__thread_id__participants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/{thread_id}/post\n  method: post\n  operationId: post_to_thread_api_v1_threads__thread_id__post_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/{thread_id}/restore\n  method: post\n  operationId: restore_thread_api_v1_threads__thread_id__restore_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/{thread_id}/baton\n  method: post\n  operationId: pass_baton_api_v1_threads__thread_id__baton_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/\n  method: get\n  operationId:\
  \ list_tasks_api_v1_tasks__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks/\n  method: post\n  operationId: create_task_api_v1_tasks__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/count\n  method: get\n  operationId: get_task_count_api_v1_tasks_count_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks/deleted\n  method: get\n  operationId: list_deleted_tasks_api_v1_tasks_deleted_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks/{task_id}/\n  method: get\n  operationId: get_task_api_v1_tasks__task_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks/{task_id}/\n  method: put\n  operationId: update_task_api_v1_tasks__task_id___put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task_id}/\n  method: delete\n  operationId: delete_task_api_v1_tasks__task_id___delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task_id}/restore\n  method: post\n  operationId: restore_task_api_v1_tasks__task_id__restore_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task_id}/status/\n  method: patch\n  operationId: change_task_status_api_v1_tasks__task_id__status__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/task-statuses/\n  method: get\n  operationId: list_task_statuses_api_v1_task_statuses__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/login\n  method: post\n  operationId: login_api_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: logout_api_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/refresh\n  method: post\n  operationId: refresh_token_api_auth_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/me\n  method: get\n  operationId: get_me_api_auth_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/me/connect-welcome/dismiss\n  method: post\n  operationId: dismiss_connect_welcome_api_auth_me_connect_welcome_dismiss_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/me/getting-started/viewed\n  method: post\n  operationId: mark_getting_started_viewed_api_auth_me_getting_started_viewed_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/me/hq-promo/dismiss\n  method: post\n  operationId: dismiss_hq_promo_api_auth_me_hq_promo_dismiss_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/api-keys/active\n  method: get\n  operationId: get_active_api_keys_api_auth_api_keys_active_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/api-keys\n  method: get\n  operationId: list_api_keys_api_auth_api_keys_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/api-keys\n  method: post\n  operationId: create_api_key_api_auth_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_api_auth_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/saas/account-registration/status\n\
  \  method: get\n  operationId: account_registration_status_api_saas_account_registration_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/register\n  method: post\n  operationId: register_account_api_saas_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/login-identifier/request\n  method: post\n  operationId: request_login_identifier_api_saas_login_identifier_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/saas/first-login\n  method: get\n  operationId: get_first_login_state_api_saas_first_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/first-login/complete\n  method: post\n  operationId: complete_first_login_api_saas_first_login_complete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/password-reset/request\n  method: post\n  operationId: request_password_reset_api_saas_password_reset_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/saas/password-reset/confirm\n  method: post\n  operationId: confirm_password_reset_api_saas_password_reset_confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/saas/email-change/request\n  method: post\n  operationId: request_email_change_api_saas_email_change_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/saas/email-change/confirm\n  method: post\n  operationId: confirm_email_change_api_saas_email_change_confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/email-change/cancel\n  method: post\n  operationId: cancel_email_change_api_saas_email_change_cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/account/cancel-deletion\n  method: post\n  operationId: cancel_deletion_api_saas_account_cancel_deletion_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/account/request-deletion\n  method: post\n  operationId: request_deletion_api_saas_account_request_deletion_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/account/confirm-deletion\n  method: post\n  operationId: confirm_deletion_api_saas_account_confirm_deletion_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/saas/account/status\n  method: get\n  operationId: get_deletion_status_api_saas_account_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/legal/accept\n  method: post\n  operationId: accept_legal_documents_api_saas_legal_accept_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/auth/social/google/start\n  method: get\n  operationId: google_start_api_saas_auth_social_google_start_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/github/start\n  method: get\n\
  \  operationId: github_start_api_saas_auth_social_github_start_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/google/callback\n  method: get\n  operationId: google_callback_api_saas_auth_social_google_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/github/callback\n  method: get\n  operationId: github_callback_api_saas_auth_social_github_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/complete-signup\n  method: post\n  operationId: complete_signup_api_saas_auth_social_complete_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/auth/social/{provider}/connect\n  method: get\n  operationId: connect_start_api_saas_auth_social__provider__connect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/{provider}/callback/connect\n  method: get\n  operationId: connect_callback_api_saas_auth_social__provider__callback_connect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/{provider}/connect/callback\n  method: get\n  operationId: connect_callback_api_saas_auth_social__provider__connect_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/social/confirm-link\n  method: post\n  operationId: confirm_link_api_saas_auth_social_confirm_link_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/auth/identities\n  method: get\n  operationId: list_identities_api_saas_auth_identities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saas/auth/identities/{provider}/disconnect\n  method: post\n  operationId: disconnect_identity_api_saas_auth_identities__provider__disconnect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/saas/auth/set-initial-password\n  method: post\n  operationId: set_initial_password_api_saas_auth_set_initial_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/authorize\n  method: post\n  operationId: authorize_api_oauth_authorize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/token\n \
  \ method: post\n  operationId: token_api_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/refresh\n  method: post\n  operationId: refresh_api_oauth_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/.well-known/oauth-authorization-server\n  method: get\n  operationId: oauth_metadata_api_oauth__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/oauth/register\n  method: post\n  operationId: register_client_api_oauth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/client-info\n  method: get\n  operationId: consent_client_info_api_oauth_client_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oauth/revoke\n  method: post\n  operationId: revoke_api_oauth_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: oauth_metadata_root_mirror__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: oauth_protected_resource_metadata__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp-server-info\n  method: get\n  operationId: mcp_server_info__well_known_mcp_server_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{user_id}\n  method: get\n  operationId: get_user_api_v1_users__user_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{user_id}\n  method: put\n  operationId: update_user_api_v1_users__user_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{user_id}/password\n  method: put\n  operationId: change_password_api_v1_users__user_id__password_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/giljo-ai/agentic-access/giljo-ai-agentic-access.yml
summary_line: 76 operations · 42 acting · 4 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Agents
- Collaboration
- Platform
---
