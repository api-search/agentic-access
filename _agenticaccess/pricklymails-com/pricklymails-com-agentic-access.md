---
acting_count: 74
action_class_counts:
  acting: 74
  connected: 58
api_specs:
- filename: pricklymails-com-account-api-openapi.yml
  format: yaml
  label: pricklymails-com Account API
  slug: pricklymails-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-account-api-openapi.yml
- filename: pricklymails-com-agents-api-openapi.yml
  format: yaml
  label: pricklymails-com Agents API
  slug: pricklymails-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-agents-api-openapi.yml
- filename: pricklymails-com-api-keys-api-openapi.yml
  format: yaml
  label: pricklymails-com API Keys API
  slug: pricklymails-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-api-keys-api-openapi.yml
- filename: pricklymails-com-auth-api-openapi.yml
  format: yaml
  label: pricklymails-com Auth API
  slug: pricklymails-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-auth-api-openapi.yml
- filename: pricklymails-com-batches-api-openapi.yml
  format: yaml
  label: pricklymails-com Batches API
  slug: pricklymails-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-batches-api-openapi.yml
- filename: pricklymails-com-billing-api-openapi.yml
  format: yaml
  label: pricklymails-com Billing API
  slug: pricklymails-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-billing-api-openapi.yml
- filename: pricklymails-com-config-api-openapi.yml
  format: yaml
  label: pricklymails-com Config API
  slug: pricklymails-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-config-api-openapi.yml
- filename: pricklymails-com-jobs-api-openapi.yml
  format: yaml
  label: pricklymails-com Jobs API
  slug: pricklymails-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-jobs-api-openapi.yml
- filename: pricklymails-com-notifications-api-openapi.yml
  format: yaml
  label: pricklymails-com Notifications API
  slug: pricklymails-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-notifications-api-openapi.yml
- filename: pricklymails-com-oauth-api-openapi.yml
  format: yaml
  label: pricklymails-com OAuth API
  slug: pricklymails-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-oauth-api-openapi.yml
- filename: pricklymails-com-sessions-api-openapi.yml
  format: yaml
  label: pricklymails-com Sessions API
  slug: pricklymails-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-sessions-api-openapi.yml
- filename: pricklymails-com-stats-api-openapi.yml
  format: yaml
  label: pricklymails-com Stats API
  slug: pricklymails-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-stats-api-openapi.yml
- filename: pricklymails-com-subscription-api-openapi.yml
  format: yaml
  label: pricklymails-com Subscription API
  slug: pricklymails-com-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-subscription-api-openapi.yml
- filename: pricklymails-com-verification-api-openapi.yml
  format: yaml
  label: pricklymails-com Verification API
  slug: pricklymails-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-verification-api-openapi.yml
- filename: pricklymails-com-wallet-api-openapi.yml
  format: yaml
  label: pricklymails-com Wallet API
  slug: pricklymails-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-wallet-api-openapi.yml
- filename: pricklymails-com-webhooks-api-openapi.yml
  format: yaml
  label: pricklymails-com Webhooks API
  slug: pricklymails-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 58
  safety-critical: 14
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 14
kind: agentic-access
layout: agentic-access
method: generated
name: Pricklymails Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/agents/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/agents/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/keys/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/keys/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/notifications/seen
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/notifications/seen
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/users/me/2fa/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/users/me/2fa/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/users/me/sessions/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/users/me/sessions/{uuid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/resend-confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/resend-confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/{uuid}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/{uuid}/test
operation_count: 132
overview: 'pricklymails-com exposes 132 API operations that an AI agent could call, of which 74 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 58 read, 54 write, 6 physical, and 14 safety-critical.


  14 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pricklymails-com
provider_slug: pricklymails-com
slug: pricklymails-com-agentic-access
source_filename: pricklymails-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/pricklymails-com-openapi.json, openapi/pricklymails-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 132\n  by_action_class:\n    connected: 58\n    acting: 74\n  by_consequence:\n    read: 58\n    write: 54\n    safety-critical: 14\n    physical: 6\n  human_in_the_loop_required: 14\noperations:\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorization_server_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: list_agents\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  operationId: create_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{uuid}\n  method: get\n  operationId: get_agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{uuid}\n  method: delete\n  operationId: revoke_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/auth/2fa/verify\n  method: post\n  operationId: verify_2fa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/confirm\n  method: post\n  operationId: confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/forgot-password\n  method: post\n  operationId: forgot_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/refresh\n  method: post\n  operationId: refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/resend-confirmation\n  method: post\n  operationId: resend_confirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/reset-password\n  method: post\n  operationId: reset_password\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/signup-preview\n  method: post\n  operationId: signup_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify-email-change\n  method: post\n  operationId: verify_email_change\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/batches\n  method: get\n  operationId: list_batches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batches\n  method: post\n  operationId: submit_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batches/{uuid}\n  method: get\n  operationId: get_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batches/{uuid}/emails\n  method: post\n  operationId: append_batch_emails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batches/{uuid}/results\n  method: get\n  operationId: get_batch_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/checkout\n  method: post\n  operationId: create_checkout_session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/portal\n  method: post\n  operationId: create_billing_portal_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config\n  method: get\n  operationId: get_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs\n  method: get\n  operationId: list_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs/{uuid}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: get\n  operationId: list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/me\n  method: get\n  operationId: get_current_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{uuid}\n  method: get\n  operationId: get_api_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{uuid}\n  method: delete\n  operationId: revoke_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/keys/{uuid}\n  method: patch\n  operationId: update_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications\n  method: get\n  operationId: list_notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/seen\n  method: post\n  operationId: mark_notifications_seen\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/stats/overview\n  method: get\n  operationId: get_stats_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats/summary\n  method: get\n  operationId: get_public_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subscription\n  method: get\n  operationId: get_subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/users/me/2fa\n  method: get\n  operationId: get_2fa_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/2fa/disable\n  method: post\n  operationId: disable_2fa\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/users/me/2fa/enable\n  method: post\n  operationId: enable_2fa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/users/me/2fa/verify-setup\n  method: post\n  operationId: verify_2fa_setup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/locale\n  method: patch\n  operationId: change_locale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/sessions\n  method: get\n  operationId: list_sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/sessions/{uuid}\n  method: delete\n\
  \  operationId: revoke_session\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/users/{uuid}\n  method: get\n  operationId: get_user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{uuid}\n  method: delete\n  operationId: delete_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{uuid}/email\n  method: patch\n  operationId: change_email\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{uuid}/password\n  method: patch\n  operationId: change_password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify\n  method: post\n  operationId: submit_verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify/{uuid}\n  method:\
  \ get\n  operationId: get_verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet\n  method: get\n  operationId: get_wallet_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet/balance-history\n  method: get\n  operationId: get_balance_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet/transactions\n  method: get\n  operationId: list_wallet_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet/transactions/grouped\n  method: get\n  operationId: list_wallet_transaction_groups\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: get\n  operationId: list_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: post\n  operationId: create_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{uuid}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{uuid}\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{uuid}\n  method: patch\n  operationId: update_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{uuid}/deliveries\n  method: get\n  operationId: list_webhook_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{uuid}/test\n  method: post\n  operationId: test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize/consent\n  method: post\n  operationId: authorize_consent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/register\n  method: post\n  operationId: register_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorization_server_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: list_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n\
  \  method: post\n  operationId: create_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{uuid}\n  method: get\n  operationId: get_agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{uuid}\n  method: delete\n  operationId: revoke_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/2fa/verify\n  method: post\n  operationId: verify_2fa\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/confirm\n  method: post\n  operationId: confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/forgot-password\n  method: post\n  operationId: forgot_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n \
  \   audit: required\n- path: /api/auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/refresh\n  method: post\n  operationId: refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/auth/register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/resend-confirmation\n  method: post\n  operationId: resend_confirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/reset-password\n  method: post\n  operationId: reset_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/signup-preview\n  method: post\n  operationId: signup_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify-email-change\n  method: post\n  operationId: verify_email_change\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batches\n  method: get\n  operationId: list_batches\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batches\n  method: post\n  operationId: submit_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batches/{uuid}\n  method: get\n  operationId: get_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batches/{uuid}/emails\n  method: post\n  operationId: append_batch_emails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batches/{uuid}/results\n  method: get\n  operationId: get_batch_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/checkout\n  method: post\n  operationId: create_checkout_session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/portal\n  method: post\n  operationId: create_billing_portal_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config\n  method: get\n  operationId: get_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs\n  method: get\n  operationId: list_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs/{uuid}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: get\n  operationId: list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/me\n  method: get\n  operationId: get_current_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{uuid}\n  method: get\n  operationId: get_api_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{uuid}\n  method: delete\n  operationId: revoke_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/keys/{uuid}\n  method: patch\n  operationId: update_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications\n  method: get\n  operationId: list_notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/seen\n  method: post\n  operationId: mark_notifications_seen\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n   \
  \   human-in-the-loop: required\n    audit: required\n- path: /api/stats/overview\n  method: get\n  operationId: get_stats_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats/summary\n  method: get\n  operationId: get_public_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subscription\n  method: get\n  operationId: get_subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/2fa\n  method: get\n  operationId: get_2fa_status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/2fa/disable\n  method: post\n  operationId: disable_2fa\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/users/me/2fa/enable\n  method: post\n  operationId: enable_2fa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/2fa/verify-setup\n  method: post\n  operationId: verify_2fa_setup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/locale\n  method: patch\n  operationId: change_locale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/sessions\n  method: get\n  operationId: list_sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (37 KB total) ---\n# Full source: https://artifacts.apis.io/pricklymails-com/agentic-access/pricklymails-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/pricklymails-com/agentic-access/pricklymails-com-agentic-access.yml
summary_line: 132 operations · 74 acting · 14 human-in-the-loop
tags:
- Email Verification
- Software-as-a-Service
- Data Validation
- EU-hosted
---
