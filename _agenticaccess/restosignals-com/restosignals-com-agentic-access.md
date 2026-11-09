---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 15
api_specs:
- filename: restosignals-com-account-api-openapi.yml
  format: yaml
  label: restosignals-com Account API
  slug: restosignals-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-account-api-openapi.yml
- filename: restosignals-com-auth-api-openapi.yml
  format: yaml
  label: restosignals-com Auth API
  slug: restosignals-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-auth-api-openapi.yml
- filename: restosignals-com-billing-api-openapi.yml
  format: yaml
  label: restosignals-com Billing API
  slug: restosignals-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-billing-api-openapi.yml
- filename: restosignals-com-config-api-openapi.yml
  format: yaml
  label: restosignals-com Config API
  slug: restosignals-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-config-api-openapi.yml
- filename: restosignals-com-export-api-openapi.yml
  format: yaml
  label: restosignals-com Export API
  slug: restosignals-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-export-api-openapi.yml
- filename: restosignals-com-health-api-openapi.yml
  format: yaml
  label: restosignals-com Health API
  slug: restosignals-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-health-api-openapi.yml
- filename: restosignals-com-keys-api-openapi.yml
  format: yaml
  label: restosignals-com Keys API
  slug: restosignals-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-keys-api-openapi.yml
- filename: restosignals-com-mcp-api-openapi.yml
  format: yaml
  label: restosignals-com MCP API
  slug: restosignals-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-mcp-api-openapi.yml
- filename: restosignals-com-me-api-openapi.yml
  format: yaml
  label: restosignals-com Me API
  slug: restosignals-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-me-api-openapi.yml
- filename: restosignals-com-openings-api-openapi.yml
  format: yaml
  label: restosignals-com Openings API
  slug: restosignals-com-openings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-openings-api-openapi.yml
- filename: restosignals-com-register-api-openapi.yml
  format: yaml
  label: restosignals-com Register API
  slug: restosignals-com-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-register-api-openapi.yml
- filename: restosignals-com-signals-api-openapi.yml
  format: yaml
  label: restosignals-com Signals API
  slug: restosignals-com-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-signals-api-openapi.yml
- filename: restosignals-com-usage-api-openapi.yml
  format: yaml
  label: restosignals-com Usage API
  slug: restosignals-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-usage-api-openapi.yml
- filename: restosignals-com-webhooks-api-openapi.yml
  format: yaml
  label: restosignals-com Webhooks API
  slug: restosignals-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/restosignals-com/openapi/restosignals-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  safety-critical: 2
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Restosignals Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/keys/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/confirm/resend
operation_count: 31
overview: 'restosignals-com exposes 31 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: restosignals-com
provider_slug: restosignals-com
slug: restosignals-com-agentic-access
source_filename: restosignals-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/restosignals-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 15\n    acting: 16\n  by_consequence:\n    read: 15\n    write: 13\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config\n  method: get\n  operationId: config_v1_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /auth/signup\n  method: post\n  operationId: signup_auth_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/confirm\n  method: get\n  operationId: auth_confirm_auth_confirm_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/confirm/resend\n  method: post\n  operationId: confirm_resend_auth_confirm_resend_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /webhooks/inbound\n  method: post\n  operationId: inbound_webhook_webhooks_inbound_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/forgot\n  method: post\n  operationId: forgot_password_auth_forgot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/reset\n  method: post\n  operationId: reset_password_auth_reset_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logout_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/register\n  method: post\n  operationId: register_anonymous_v1_register_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: get\n  operationId: me_v1_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: create_key_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/revoke\n  method: post\n  operationId: revoke_key_v1_keys_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: account_v1_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/subscribe\n  method: post\n  operationId: subscribe_billing_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /billing/topup\n  method: post\n  operationId: topup_billing_topup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/razorpay\n  method: post\n  operationId: razorpay_webhook_webhooks_razorpay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcp_descriptor_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp_post_mcp_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/openings\n  method: get\n  operationId: openings_v1_openings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/openings\n  method: get\n  operationId: app_openings_v1_app_openings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/export\n  method: get\n  operationId: app_export_v1_app_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/coverage\n  method:\
  \ get\n  operationId: app_coverage_v1_app_coverage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openings/latest\n  method: get\n  operationId: openings_latest_v1_openings_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: signals_v1_signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: list_webhooks_v1_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: register_webhook_v1_webhooks_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{wid}\n  method: delete\n  operationId: delete_webhook_v1_webhooks__wid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: get\n  operationId: export_v1_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/restosignals-com/agentic-access/restosignals-com-agentic-access.yml
summary_line: 31 operations · 16 acting · 2 human-in-the-loop
tags:
- Restaurant
- Data
- MCP
- Lead Generation
---
