---
acting_count: 60
action_class_counts:
  acting: 60
  connected: 121
api_specs:
- filename: lumify-ai-admin-api-openapi.yml
  format: yaml
  label: lumify-ai Admin API
  slug: lumify-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-admin-api-openapi.yml
- filename: lumify-ai-agent-api-openapi.yml
  format: yaml
  label: lumify-ai Agent API
  slug: lumify-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-agent-api-openapi.yml
- filename: lumify-ai-app-api-openapi.yml
  format: yaml
  label: lumify-ai App API
  slug: lumify-ai-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-app-api-openapi.yml
- filename: lumify-ai-auth-api-openapi.yml
  format: yaml
  label: lumify-ai Auth API
  slug: lumify-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-auth-api-openapi.yml
- filename: lumify-ai-events-api-openapi.yml
  format: yaml
  label: lumify-ai Events API
  slug: lumify-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-events-api-openapi.yml
- filename: lumify-ai-grade-api-openapi.yml
  format: yaml
  label: lumify-ai Grade API
  slug: lumify-ai-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-grade-api-openapi.yml
- filename: lumify-ai-health-api-openapi.yml
  format: yaml
  label: lumify-ai Health API
  slug: lumify-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-health-api-openapi.yml
- filename: lumify-ai-mcp-api-openapi.yml
  format: yaml
  label: lumify-ai MCP API
  slug: lumify-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-mcp-api-openapi.yml
- filename: lumify-ai-oauth-api-openapi.yml
  format: yaml
  label: lumify-ai OAuth API
  slug: lumify-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-oauth-api-openapi.yml
- filename: lumify-ai-players-api-openapi.yml
  format: yaml
  label: lumify-ai Players API
  slug: lumify-ai-players-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-players-api-openapi.yml
- filename: lumify-ai-public-api-openapi.yml
  format: yaml
  label: lumify-ai Public API
  slug: lumify-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-public-api-openapi.yml
- filename: lumify-ai-resolve-api-openapi.yml
  format: yaml
  label: lumify-ai Resolve API
  slug: lumify-ai-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-resolve-api-openapi.yml
- filename: lumify-ai-sports-api-openapi.yml
  format: yaml
  label: lumify-ai Sports API
  slug: lumify-ai-sports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-sports-api-openapi.yml
- filename: lumify-ai-teams-api-openapi.yml
  format: yaml
  label: lumify-ai Teams API
  slug: lumify-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-teams-api-openapi.yml
- filename: lumify-ai-trial-api-openapi.yml
  format: yaml
  label: lumify-ai Trial API
  slug: lumify-ai-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-trial-api-openapi.yml
- filename: lumify-ai-webhooks-api-openapi.yml
  format: yaml
  label: lumify-ai Webhooks API
  slug: lumify-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumify-ai/openapi/lumify-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 121
  safety-critical: 6
  write: 47
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Lumify Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/bet-intelligence/kill-switch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/users/{user_id}/password-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/users/{user_id}/revoke-sessions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api-keys/{key_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/agent/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset-password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/customers/{customer_id}/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/users/{user_id}/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agent/credits/topup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/auto-recharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/payment-method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/payment-method/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /resend-verification
operation_count: 181
overview: 'lumify-ai exposes 181 API operations that an AI agent could call, of which 60 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 121 read, 47 write, 7 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lumify-ai
provider_slug: lumify-ai
slug: lumify-ai-agentic-access
source_filename: lumify-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/lumify-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 181\n  by_action_class:\n    connected: 121\n    acting: 60\n  by_consequence:\n    read: 121\n    write: 47\n    safety-critical: 6\n    physical: 7\n  human_in_the_loop_required: 6\noperations:\n- path: /v1/health\n  method: get\n  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: get\n  operationId: login_page_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /login\n  method: post\n  operationId: login_submit_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: get\n  operationId: logout_logout_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: get\n  operationId: register_page_register_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  operationId: register_submit_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /forgot-password\n  method: get\n  operationId: forgot_password_page_forgot_password_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forgot-password\n  method: post\n  operationId: forgot_password_submit_forgot_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reset-password\n  method: get\n  operationId: reset_password_page_reset_password_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /reset-password\n  method: post\n  operationId: reset_password_submit_reset_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /verify-email\n  method: get\n  operationId: verify_email_verify_email_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resend-verification\n  method: post\n  operationId: resend_verification_resend_verification_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/github/start\n  method: get\n  operationId: github_oauth_start_oauth_github_start_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/github/callback\n  method: get\n  operationId: github_oauth_callback_oauth_github_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard\n  method: get\n  operationId: dashboard_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: account_page_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /account/profile\n  method: post\n  operationId: account_profile_update_account_profile_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/organization\n  method: post\n  operationId: account_organization_update_account_organization_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/password\n  method: post\n  operationId: account_password_change_account_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys\n  method: get\n  operationId: api_keys_page_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: api_key_create_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys/{key_id}/reveal\n  method: get\n  operationId: api_key_reveal_api_keys__key_id__reveal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api-keys/{key_id}/revoke\n  method: post\n  operationId: api_key_revoke_api_keys__key_id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing\n  method: get\n  operationId: billing_page_billing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/invoices/{invoice_id}/receipt\n  method: get\n  operationId: billing_invoice_receipt_billing_invoices__invoice_id__receipt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/auto-recharge\n  method:\
  \ post\n  operationId: billing_auto_recharge_billing_auto_recharge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/subscribe\n  method: post\n  operationId: billing_subscribe_billing_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/setup-intent\n  method: post\n  operationId: billing_setup_intent_billing_setup_intent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/payment-method\n  method: post\n  operationId: billing_attach_payment_method_billing_payment_method_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/cancel\n  method: post\n  operationId: billing_cancel_subscription_billing_cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /billing/payment-method/remove\n  method: post\n  operationId: billing_remove_payment_method_billing_payment_method_remove_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/coupon\n  method: post\n  operationId: billing_apply_coupon_billing_coupon_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal\n  method: get\n  operationId: billing_portal_billing_portal_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: usage_page_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics\n  method: get\n  operationId: analytics_page_analytics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playground\n  method: get\n  operationId: playground_page_playground_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/docs-visit\n  method: post\n  operationId: onboarding_docs_visit_onboarding_docs_visit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users\n  method: get\n  operationId: admin_users_admin_users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}/detail\n  method: get\n  operationId: admin_user_detail_admin_users__user_id__detail_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}/revoke-sessions\n  method: post\n  operationId: admin_user_revoke_sessions_admin_users__user_id__revoke_sessions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/users/{user_id}/password-reset\n  method: post\n  operationId: admin_user_password_reset_admin_users__user_id__password_reset_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/users/{user_id}/resend-verification\n  method: post\n  operationId: admin_user_resend_verification_admin_users__user_id__resend_verification_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /admin/users/{user_id}/delete\n  method: post\n  operationId: admin_user_delete_admin_users__user_id__delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/staff-role\n  method: post\n  operationId: admin_user_staff_role_admin_users__user_id__staff_role_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/rate-limit\n  method: post\n  operationId: admin_user_rate_limit_admin_users__user_id__rate_limit_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/role\n  method: post\n  operationId: admin_user_role_admin_users__user_id__role_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/toggle\n  method: post\n  operationId: admin_user_toggle_admin_users__user_id__toggle_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /admin/coupons\n  method: get\n  operationId: admin_coupons_admin_coupons_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/coupons/create\n  method: post\n  operationId: admin_coupon_create_admin_coupons_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/coupons/{coupon_id}/toggle\n  method: post\n  operationId: admin_coupon_toggle_admin_coupons__coupon_id__toggle_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/coupons/{coupon_id}/delete\n  method: post\n  operationId: admin_coupon_delete_admin_coupons__coupon_id__delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/security\n  method: get\n  operationId: admin_security_admin_security_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/plans\n  method: get\n  operationId: admin_plans_admin_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/plans/{plan_id}/update\n  method: post\n\
  \  operationId: admin_plans_update_admin_plans__plan_id__update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/plans/{plan_id}/delete\n  method: post\n  operationId: admin_plans_delete_admin_plans__plan_id__delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/settings\n  method: get\n  operationId: admin_settings_admin_settings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/settings/free-trial-daily-cap\n\
  \  method: post\n  operationId: admin_update_free_trial_daily_cap_admin_settings_free_trial_daily_cap_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/customers\n  method: get\n  operationId: admin_customers_admin_customers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/customers/{customer_id}/detail\n  method: get\n  operationId: admin_customer_detail_admin_customers__customer_id__detail_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/customers/{customer_id}/usage\n  method: get\n  operationId: admin_customer_usage_admin_customers__customer_id__usage_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/customers/{customer_id}/entitlements\n  method: post\n  operationId: admin_customer_entitlements_admin_customers__customer_id__entitlements_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/customers/{customer_id}/name\n  method: post\n  operationId: admin_customer_name_admin_customers__customer_id__name_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/customers/{customer_id}/exclude-from-analytics\n  method: post\n  operationId: admin_customer_exclude_from_analytics_admin_customers__customer_id__exclude_from_analytics_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/customers/{customer_id}/resend-verification\n  method: post\n  operationId: admin_customer_resend_verification_admin_customers__customer_id__resend_verification_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/customers/{customer_id}/delete\n\
  \  method: post\n  operationId: admin_customer_delete_admin_customers__customer_id__delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/usage\n  method: get\n  operationId: admin_usage_admin_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/usage/customer-errors\n  method: get\n  operationId: admin_usage_customer_errors_admin_usage_customer_errors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/usage/customer-activity\n  method: get\n  operationId: admin_usage_customer_activity_admin_usage_customer_activity_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/onboarding-rewards\n  method: get\n  operationId: admin_onboarding_rewards_admin_onboarding_rewards_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/performance\n  method: get\n  operationId: admin_performance_admin_performance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/pricing\n  method: get\n  operationId: admin_pricing_admin_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/pricing/create\n  method: post\n  operationId: admin_pricing_create_admin_pricing_create_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/pricing/{config_id}/toggle\n  method: post\n  operationId: admin_pricing_toggle_admin_pricing__config_id__toggle_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/pricing/{config_id}/update\n  method: post\n  operationId: admin_pricing_update_admin_pricing__config_id__update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/pricing/actuals/save\n  method: post\n  operationId: admin_pricing_actuals_save_admin_pricing_actuals_save_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/sports-schedule\n  method: get\n  operationId: admin_sports_schedule_admin_sports_schedule_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/bet-intelligence\n  method: get\n  operationId: admin_bet_intelligence_admin_bet_intelligence_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /admin/bet-intelligence/mode\n  method: post\n  operationId: admin_bet_intelligence_set_mode_admin_bet_intelligence_mode_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/bet-intelligence/kill-switch\n  method: post\n  operationId: admin_bet_intelligence_kill_switch_admin_bet_intelligence_kill_switch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/events/{event_id}\n  method: get\n  operationId: admin_event_detail_admin_events__event_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/intelligence\n  method: get\n  operationId: admin_event_intelligence_admin_events__event_id__intelligence_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/odds\n  method: get\n  operationId: admin_event_odds_admin_events__event_id__odds_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/player-props\n  method: get\n  operationId: admin_event_player_props_admin_events__event_id__player_props_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /admin/events/{event_id}/period-odds\n  method: get\n  operationId: admin_event_period_odds_admin_events__event_id__period_odds_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/team-props\n  method: get\n  operationId: admin_event_team_props_admin_events__event_id__team_props_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/splits\n  method: get\n  operationId: admin_event_splits_admin_events__event_id__splits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/stats\n  method: get\n  operationId: admin_event_stats_admin_events__event_id__stats_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/events/{event_id}/injuries\n  method: get\n  operationId: admin_event_injuries_admin_events__event_id__injuries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/predictive\n  method: get\n  operationId: admin_predictive_admin_predictive_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/predictive/status.json\n  method: get\n  operationId: admin_predictive_status_admin_predictive_status_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/job-health\n  method: get\n  operationId: admin_job_health_admin_job_health_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/job-health/status.json\n  method: get\n  operationId: admin_job_health_status_admin_job_health_status_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/job-health/attention-count.json\n  method: get\n  operationId: admin_job_health_attention_count_admin_job_health_attention_count_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/job-health/mute\n  method: post\n  operationId: admin_job_health_mute_admin_job_health_mute_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: home__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: pricing_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quickstart\n  method: get\n  operationId: docs_quickstart_quickstart_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: docs_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/guides\n  method: get\n  operationId: docs_guides_docs_guides_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/ai\n  method: get\n  operationId: docs_ai_docs_ai_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/cheat-sheet\n  method: get\n  operationId: docs_cheat_sheet_docs_cheat_sheet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/glossary\n  method: get\n  operationId: docs_glossary_docs_glossary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/player-props\n  method: get\n  operationId: docs_player_props_docs_player_props_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/best-practices\n  method: get\n  operationId: docs_best_practices_docs_best_practices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/rate-limits\n  method: get\n  operationId: docs_rate_limits_docs_rate_limits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/reference\n  method: get\n  operationId: docs_reference_docs_reference_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (51 KB total) ---\n# Full source: https://artifacts.apis.io/lumify-ai/agentic-access/lumify-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/lumify-ai/agentic-access/lumify-ai-agentic-access.yml
summary_line: 181 operations · 60 acting · 6 human-in-the-loop
tags:
- Company
- Sports
- Artificial Intelligence
- Real-Time
- Betting
---
