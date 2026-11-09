---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 30
api_specs:
- filename: twtapi-com-admin-api-openapi.yml
  format: yaml
  label: twtapi-com Admin API
  slug: twtapi-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-admin-api-openapi.yml
- filename: twtapi-com-agent-api-openapi.yml
  format: yaml
  label: twtapi-com Agent API
  slug: twtapi-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-agent-api-openapi.yml
- filename: twtapi-com-auth-api-openapi.yml
  format: yaml
  label: twtapi-com Auth API
  slug: twtapi-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-auth-api-openapi.yml
- filename: twtapi-com-captcha-api-openapi.yml
  format: yaml
  label: twtapi-com Captcha API
  slug: twtapi-com-captcha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-captcha-api-openapi.yml
- filename: twtapi-com-myapi-api-openapi.yml
  format: yaml
  label: twtapi-com Myapi API
  slug: twtapi-com-myapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-myapi-api-openapi.yml
- filename: twtapi-com-payment-api-openapi.yml
  format: yaml
  label: twtapi-com Payment API
  slug: twtapi-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-payment-api-openapi.yml
- filename: twtapi-com-twitter-api-openapi.yml
  format: yaml
  label: twtapi-com Twitter API
  slug: twtapi-com-twitter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-twitter-api-openapi.yml
- filename: twtapi-com-twtapi-backend-api-openapi.yml
  format: yaml
  label: twtapi-com TwtAPI Backend API
  slug: twtapi-com-twtapi-backend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-twtapi-backend-api-openapi.yml
consequence_counts:
  physical: 5
  read: 30
  safety-critical: 5
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Twtapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/resetPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/sendResetPasswordEmail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /myapi/resetApiKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /myapi/resetMcpKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /myapi/resetSkillKey
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/sendEmailCode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/cancel-subscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/create-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/webhook/{provider_name}
operation_count: 57
overview: 'twtapi-com exposes 57 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 17 write, 5 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: twtapi-com
provider_slug: twtapi-com
slug: twtapi-com-agentic-access
source_filename: twtapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/twtapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 30\n    acting: 27\n  by_consequence:\n    read: 30\n    physical: 5\n    write: 17\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /captcha\n  method: get\n  operationId: captcha_image_captcha_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/google/start\n  method: get\n  operationId: google_oauth_start_auth_oauth_google_start_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/google/callback\n  method: get\n  operationId: google_oauth_callback_auth_oauth_google_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/sendEmailCode\n  method: post\n  operationId: send_email_code_auth_sendEmailCode_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/register\n  method: post\n  operationId: register_auth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/getInfo\n  method: get\n  operationId: get_info_auth_getInfo_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/logout\n  method: post\n  operationId: logout_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /auth/checkCaptchaRequired\n  method: post\n  operationId: check_captcha_required_auth_checkCaptchaRequired_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/sendResetPasswordEmail\n  method: post\n  operationId: send_reset_password_email_auth_sendResetPasswordEmail_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/resetPassword\n  method: post\n  operationId: reset_password_auth_resetPassword_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/changePassword\n  method: post\n  operationId: change_password_auth_changePassword_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/order\n  method: post\n  operationId: create_order_auth_order_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /myapi/getApiKey\n  method: get\n  operationId: get_api_key_myapi_getApiKey_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/getMcpKey\n  method: get\n  operationId: get_mcp_key_myapi_getMcpKey_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/getSkillKey\n  method: get\n  operationId: get_skill_key_myapi_getSkillKey_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/resetApiKey\n  method: post\n  operationId: reset_api_key_myapi_resetApiKey_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /myapi/resetMcpKey\n  method: post\n  operationId: reset_mcp_key_myapi_resetMcpKey_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /myapi/resetSkillKey\n  method: post\n  operationId: reset_skill_key_myapi_resetSkillKey_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /myapi/dashboard\n  method: get\n  operationId: dashboard_myapi_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/status\n  method: get\n  operationId: api_status_myapi_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/orders\n  method: get\n  operationId: my_orders_myapi_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/requests\n  method: get\n  operationId: my_requests_myapi_requests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/usage\n  method: get\n  operationId: my_usage_myapi_usage_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myapi/plans\n  method: get\n  operationId: public_plans_myapi_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/twitter/{path}\n  method: get\n  operationId: proxy_api_v1_twitter__path__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/twitter/{path}\n  method: post\n  operationId: proxy_api_v1_twitter__path__get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/twitter/{path}\n\
  \  method: put\n  operationId: proxy_api_v1_twitter__path__get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/twitter/{path}\n  method: delete\n  operationId: proxy_api_v1_twitter__path__get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/twitter/{path}\n  method: patch\n  operationId: proxy_api_v1_twitter__path__get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent/tools\n  method: get\n  operationId: tools_api_v1_agent_tools_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/invoke\n  method: post\n  operationId: invoke_api_v1_agent_invoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users\n  method: get\n  operationId: list_users_admin_users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}\n  method: get\n  operationId: get_user_admin_users__user_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}/risk\n  method: get\n  operationId: get_user_risk_admin_users__user_id__risk_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}/credits\n  method: post\n  operationId: adjust_credits_admin_users__user_id__credits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/status\n  method: post\n  operationId: update_status_admin_users__user_id__status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/limits\n  method: post\n  operationId: update_limits_admin_users__user_id__limits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_id}/plan\n  method: post\n  operationId: update_user_plan_admin_users__user_id__plan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/orders\n\
  \  method: get\n  operationId: list_orders_admin_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/orders/{order_id}\n  method: get\n  operationId: get_order_admin_orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/logs\n  method: get\n  operationId: get_call_logs_admin_logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}/activity\n  method: get\n  operationId: get_user_activity_admin_users__user_id__activity_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/revenue\n  method: get\n  operationId:\
  \ revenue_stats_admin_revenue_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/stats\n  method: get\n  operationId: global_stats_admin_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/growth-funnel\n  method: get\n  operationId: growth_funnel_admin_growth_funnel_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/rapidapi-quota\n  method: get\n  operationId: rapidapi_quota_admin_rapidapi_quota_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/leak-audit\n  method: get\n  operationId: leak_audit_admin_leak_audit_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/plans\n  method: get\n  operationId: get_plans_admin_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/plans\n  method: post\n  operationId: create_plan_admin_plans_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/plans/{plan_id}\n  method: put\n  operationId: update_plan_admin_plans__plan_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/plans/{plan_id}\n  method: delete\n  operationId: delete_plan_admin_plans__plan_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/create-checkout\n  method: post\n  operationId: create_checkout_payment_create_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/webhook/{provider_name}\n  method: post\n  operationId: payment_webhook_payment_webhook__provider_name__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/status/{order_no}\n  method: get\n  operationId: payment_status_payment_status__order_no__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/cancel-subscription\n  method: post\n  operationId: cancel_subscription_payment_cancel_subscription_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/twtapi-com/agentic-access/twtapi-com-agentic-access.yml
summary_line: 57 operations · 27 acting · 5 human-in-the-loop
tags:
- Twitter
- X
- Data
- Search
- Monitoring
- Artificial Intelligence
---
