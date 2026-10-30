---
acting_count: 148
action_class_counts:
  acting: 148
  connected: 110
api_specs:
- filename: monacloud-apps-api-openapi.yml
  format: yaml
  label: The MONA Group Apps API
  slug: monacloud-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-apps-api-openapi.yml
- filename: monacloud-auth-api-openapi.yml
  format: yaml
  label: The MONA Group Auth API
  slug: monacloud-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-auth-api-openapi.yml
- filename: monacloud-billing-api-openapi.yml
  format: yaml
  label: The MONA Group Billing API
  slug: monacloud-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-billing-api-openapi.yml
- filename: monacloud-databases-api-openapi.yml
  format: yaml
  label: The MONA Group Databases API
  slug: monacloud-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-databases-api-openapi.yml
- filename: monacloud-jobs-api-openapi.yml
  format: yaml
  label: The MONA Group Jobs API
  slug: monacloud-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-jobs-api-openapi.yml
- filename: monacloud-lxc-api-openapi.yml
  format: yaml
  label: The MONA Group Lxc API
  slug: monacloud-lxc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-lxc-api-openapi.yml
- filename: monacloud-prices-api-openapi.yml
  format: yaml
  label: The MONA Group Prices API
  slug: monacloud-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-prices-api-openapi.yml
- filename: monacloud-sandbox-api-openapi.yml
  format: yaml
  label: The MONA Group Sandbox API
  slug: monacloud-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-sandbox-api-openapi.yml
- filename: monacloud-services-api-openapi.yml
  format: yaml
  label: The MONA Group Services API
  slug: monacloud-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/openapi/monacloud-services-api-openapi.yml
consequence_counts:
  physical: 19
  read: 110
  safety-critical: 21
  write: 108
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 21
kind: agentic-access
layout: agentic-access
method: generated
name: Monacloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/apps/{app_id}/auto-deploy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/check-otp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/check-otp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/stop-impersonation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/stop-impersonation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lxc/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lxc/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sandbox/lxc/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sandbox/lxc/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sandbox/services/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sandbox/services/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/services/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/services/{service_id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/apps
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/apps/{app_id}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/apps/{app_id}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/apps/{app_id}/env
operation_count: 258
overview: 'The MONA Group exposes 258 API operations that an AI agent could call, of which 148 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 110 read, 108 write, 19 physical, and 21 safety-critical.


  21 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The MONA Group
provider_slug: monacloud
slug: monacloud-agentic-access
source_filename: monacloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/monacloud-api-openapi.json, openapi/monacloud-vn-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 258\n  by_action_class:\n    acting: 148\n    connected: 110\n  by_consequence:\n    write: 108\n    safety-critical: 21\n    physical: 19\n    read: 110\n  human_in_the_loop_required: 21\noperations:\n- path: /api/auth/login\n  method: post\n  operationId: api_login_api_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/check-otp\n\
  \  method: post\n  operationId: api_check_otp_api_auth_check_otp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/refresh\n  method: post\n  operationId: api_refresh_access_token_api_auth_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/identify\n  method: post\n  operationId: api_identify_email_api_auth_identify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/register/verify\n  method: post\n  operationId: api_register_verify_api_auth_register_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/reset/start\n  method: post\n  operationId: api_reset_start_api_auth_reset_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n   \
  \ audit: required\n- path: /api/auth/reset/verify\n  method: post\n  operationId: api_reset_verify_api_auth_reset_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/providers\n  method: get\n  operationId: api_auth_providers_api_auth_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: get\n  operationId: api_me_api_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/referral\n  method: get\n  operationId: api_me_referral_api_me_referral_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/affiliate\n  method: get\n  operationId: api_me_affiliate_api_me_affiliate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/affiliate/commissions\n  method: get\n  operationId: api_me_affiliate_commissions_api_me_affiliate_commissions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/affiliate/referrals\n  method: get\n  operationId: api_me_affiliate_referrals_api_me_affiliate_referrals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/affiliate/settings\n  method: put\n  operationId: api_me_affiliate_settings_api_me_affiliate_settings_put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/affiliate/payouts\n  method: get\n  operationId: api_me_affiliate_payouts_api_me_affiliate_payouts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/affiliate/payouts\n  method: post\n  operationId: api_me_affiliate_request_payout_api_me_affiliate_payouts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/referral/claim\n  method: post\n  operationId: api_me_referral_claim_api_me_referral_claim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/affiliate/click\n  method: post\n  operationId: api_public_affiliate_click_api_public_affiliate_click_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/credit-grants\n  method: get\n  operationId: api_me_credit_grants_api_me_credit_grants_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/logout\n  method: post\n  operationId: api_logout_api_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dashboard\n  method: get\n  operationId: api_dashboard_api_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys\n  method: get\n  operationId: api_list_keys_api_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys\n\
  \  method: post\n  operationId: api_create_key_api_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/api-keys/{key_id}\n  method: delete\n  operationId: api_revoke_key_api_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/payments/vietqr\n  method: post\n  operationId: api_create_vietqr_invoice_api_payments_vietqr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments\n  method: get\n  operationId: api_list_payments_api_payments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{payment_id}\n  method: get\n  operationId: api_get_payment_api_payments__payment_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/payments\n  method: post\n  operationId: payment_webhook_api_webhooks_payments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/prices\n  method: get\n  operationId: api_public_prices_api_prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capabilities\n  method: get\n  operationId: api_public_capabilities_api_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/packages\n  method: get\n  operationId: api_public_packages_api_packages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/plans\n  method: get\n  operationId: api_public_plans_api_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credit-codes/redeem\n  method: post\n  operationId: api_redeem_credit_code_api_credit_codes_redeem_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/subscriptions\n  method: get\n  operationId: api_list_subscriptions_api_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/services/{service_id}/subscription\n  method: post\n  operationId: api_change_subscription_api_services__service_id__subscription_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices\n  method: get\n  operationId: api_list_invoices_api_invoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices/{invoice_id}.pdf\n  method: get\n  operationId: api_invoice_pdf_api_invoices__invoice_id__pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lxc\n  method: post\n  operationId: create_lxc_api_lxc_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/sandbox/lxc\n  method: post\n  operationId: create_lxc_api_sandbox_lxc_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/databases\n  method: post\n  operationId: create_database_api_databases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/databases\n  method: post\n  operationId: create_database_api_sandbox_databases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/databases/{service_id}/databases\n  method: post\n  operationId: add_database_to_instance_api_databases__service_id__databases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/databases/{service_id}/databases/{db_name}/password\n  method: post\n  operationId: regenerate_database_password_api_databases__service_id__databases__db_name__password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/databases/{service_id}/databases/{db_name}\n  method: delete\n  operationId: delete_database_on_instance_api_databases__service_id__databases__db_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/jobs/{job_id}\n  method: get\n  operationId: get_job_api_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/jobs/{job_id}\n  method: get\n  operationId: get_job_api_sandbox_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs\n  method: get\n  operationId: list_jobs_api_jobs_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/jobs\n  method: get\n  operationId: list_jobs_api_sandbox_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs/{job_id}/retry\n  method: post\n  operationId: retry_job_api_jobs__job_id__retry_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/services\n  method: get\n  operationId: list_services_api_services_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/services\n  method: get\n  operationId: list_services_api_sandbox_services_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/services/{service_id}\n  method: get\n  operationId: get_service_api_services__service_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/services/{service_id}\n  method: delete\n  operationId: delete_service_api_services__service_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/services/{service_id}\n  method:\
  \ get\n  operationId: get_service_api_sandbox_services__service_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/services/{service_id}\n  method: delete\n  operationId: delete_service_api_sandbox_services__service_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/services/{service_id}/credentials\n  method: get\n  operationId: get_service_credentials_api_services__service_id__credentials_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/services/{service_id}/console\n  method: get\n  operationId: service_console_api_services__service_id__console_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/services/{service_id}/console\n  method: get\n  operationId: service_console_api_sandbox_services__service_id__console_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/services/{service_id}/stop\n  method: post\n  operationId: stop_service_api_services__service_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/sandbox/services/{service_id}/stop\n  method: post\n  operationId: stop_service_api_sandbox_services__service_id__stop_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/services/{service_id}/start\n  method: post\n  operationId: start_service_api_services__service_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/services/{service_id}/start\n  method: post\n  operationId: start_service_api_sandbox_services__service_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lxc/{service_id}/stop\n  method: post\n  operationId: stop_lxc_api_lxc__service_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/sandbox/lxc/{service_id}/stop\n  method: post\n  operationId: stop_lxc_api_sandbox_lxc__service_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /api/lxc/{service_id}/start\n  method: post\n  operationId: start_lxc_api_lxc__service_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/lxc/{service_id}/start\n  method: post\n  operationId: start_lxc_api_sandbox_lxc__service_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lxc/{service_id}\n  method: delete\n  operationId: delete_lxc_api_lxc__service_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/lxc/{service_id}\n  method: delete\n  operationId: delete_lxc_api_sandbox_lxc__service_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lxc/{service_id}/resize\n  method: post\n  operationId: resize_lxc_api_lxc__service_id__resize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lxc/{service_id}/rebuild\n  method:\
  \ post\n  operationId: rebuild_lxc_api_lxc__service_id__rebuild_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/lxc/{service_id}/rebuild\n  method: post\n  operationId: rebuild_lxc_api_sandbox_lxc__service_id__rebuild_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/services/{service_id}/rebuild\n  method: post\n  operationId: rebuild_service_api_services__service_id__rebuild_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/services/{service_id}/rebuild\n  method: post\n  operationId: rebuild_service_api_sandbox_services__service_id__rebuild_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/guide\n  method: get\n  operationId: api_guide_api_guide_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/client-scripts\n  method: get\n  operationId: api_client_scripts_api_client_scripts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quota\n  method: get\n  operationId: api_get_quota_api_quota_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quota-requests\n  method: get\n  operationId: api_list_my_quota_requests_api_quota_requests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quota-requests\n  method: post\n  operationId: api_create_quota_request_api_quota_requests_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/stop-impersonation\n  method: post\n  operationId: api_stop_impersonation_api_auth_stop_impersonation_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/app-hosts\n  method: get\n  operationId: list_app_hosts_api_app_hosts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/app-hosts\n  method: post\n  operationId: create_app_host_api_app_hosts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps\n  method: get\n  operationId: list_apps_api_apps_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps\n  method: post\n  operationId: create_app_api_apps_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/upload\n  method: post\n  operationId: upload_app_api_apps__app_id__upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}\n  method: get\n  operationId: get_app_api_apps__app_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{app_id}\n  method: delete\n  operationId: delete_app_api_apps__app_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/auto-deploy\n  method: post\n  operationId: set_auto_deploy_api_apps__app_id__auto_deploy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/apps/{app_id}/auto-deploy\n\
  \  method: get\n  operationId: get_auto_deploy_api_apps__app_id__auto_deploy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{app_id}/webhook\n  method: post\n  operationId: github_webhook_api_apps__app_id__webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/deploy\n  method: post\n  operationId: deploy_app_api_apps__app_id__deploy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/deployments\n  method: get\n  operationId: app_deployments_api_apps__app_id__deployments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{app_id}/rollback\n  method: post\n  operationId: rollback_app_api_apps__app_id__rollback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/env\n  method: put\n  operationId: update_env_api_apps__app_id__env_put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/domains\n  method: post\n  operationId: add_domain_api_apps__app_id__domains_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{app_id}/logs\n  method: get\n  operationId: app_logs_api_apps__app_id__logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bases\n  method: get\n  operationId: list_bases_api_bases_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bases\n  method: post\n  operationId: create_base_api_bases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bases/{base_id}\n  method: get\n  operationId: get_base_api_bases__base_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (82 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/agentic-access/monacloud-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monacloud/refs/heads/main/agentic-access/monacloud-agentic-access.yml
summary_line: 258 operations · 148 acting · 21 human-in-the-loop
tags:
- Cloud
- Hosting
- Developer Tools
- Vietnamese
- Artificial Intelligence
---
