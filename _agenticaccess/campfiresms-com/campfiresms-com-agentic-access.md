---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 9
api_specs:
- filename: campfiresms-com-auth-api-openapi.yml
  format: yaml
  label: Campfire SMS Auth API
  slug: campfiresms-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-auth-api-openapi.yml
- filename: campfiresms-com-bridges-api-openapi.yml
  format: yaml
  label: Campfire SMS Bridges API
  slug: campfiresms-com-bridges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-bridges-api-openapi.yml
- filename: campfiresms-com-credential-api-openapi.yml
  format: yaml
  label: Campfire SMS Credential API
  slug: campfiresms-com-credential-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-credential-api-openapi.yml
- filename: campfiresms-com-enrollment-api-openapi.yml
  format: yaml
  label: Campfire SMS Enrollment API
  slug: campfiresms-com-enrollment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-enrollment-api-openapi.yml
- filename: campfiresms-com-health-api-openapi.yml
  format: yaml
  label: Campfire SMS Health API
  slug: campfiresms-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-health-api-openapi.yml
- filename: campfiresms-com-installations-api-openapi.yml
  format: yaml
  label: Campfire SMS Installations API
  slug: campfiresms-com-installations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-installations-api-openapi.yml
- filename: campfiresms-com-join-api-openapi.yml
  format: yaml
  label: Campfire SMS Join API
  slug: campfiresms-com-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-join-api-openapi.yml
- filename: campfiresms-com-login-api-openapi.yml
  format: yaml
  label: Campfire SMS Login API
  slug: campfiresms-com-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-login-api-openapi.yml
- filename: campfiresms-com-public-api-openapi.yml
  format: yaml
  label: Campfire SMS Public API
  slug: campfiresms-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-public-api-openapi.yml
- filename: campfiresms-com-setup-api-openapi.yml
  format: yaml
  label: Campfire SMS Setup API
  slug: campfiresms-com-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-setup-api-openapi.yml
- filename: campfiresms-com-webhooks-api-openapi.yml
  format: yaml
  label: Campfire SMS Webhooks API
  slug: campfiresms-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  safety-critical: 1
  write: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Campfiresms Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/setup/credentials/{credential_id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bridges/{bridge_id}/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/enrollment/test-sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public/checkout
operation_count: 42
overview: 'Campfire SMS exposes 42 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 29 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Campfire SMS
provider_slug: campfiresms-com
slug: campfiresms-com-agentic-access
source_filename: campfiresms-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/campfiresms-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 9\n    acting: 33\n  by_consequence:\n    read: 9\n    write: 29\n    physical: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /join\n  method: get\n  operationId: join_join_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrollment/begin\n  method: post\n  operationId: begin_signup_v1_enrollment_begin_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrollment/verify\n  method: post\n  operationId: verify_phone_v1_enrollment_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrollment/pin\n  method: post\n  operationId: set_enrollment_pin_v1_enrollment_pin_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrollment/install\n  method: post\n  operationId: create_install_v1_enrollment_install_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrollment/install-command\n  method: post\n  operationId: get_install_command_v1_enrollment_install_command_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrollment/install-status\n  method: post\n  operationId: check_install_status_v1_enrollment_install_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrollment/test-sms\n  method: post\n\
  \  operationId: send_test_sms_v1_enrollment_test_sms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/installations/consume\n  method: post\n  operationId: consume_install_v1_installations_consume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/checkout\n  method: post\n  operationId: create_checkout_v1_public_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setup\n  method: get\n  operationId: setup_setup_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/setup/pin\n  method: post\n  operationId: set_setup_pin_v1_setup_pin_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/pin/update\n  method: post\n  operationId: update_setup_pin_v1_setup_pin_update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/verification/start\n  method: post\n  operationId: start_setup_verification_v1_setup_verification_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/verification/check\n  method: post\n  operationId: check_setup_verification_v1_setup_verification_check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credentials\n\
  \  method: post\n  operationId: issue_installation_credential_v1_setup_credentials_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credentials/{credential_id}/revoke\n  method: post\n  operationId: revoke_installation_credential_v1_setup_credentials__credential_id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/setup/grok-wake\n  method: post\n  operationId: configure_account_grok_wake_v1_setup_grok_wake_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credentials/{credential_id}/grok-wake\n  method: post\n  operationId: configure_grok_wake_v1_setup_credentials__credential_id__grok_wake_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credentials/{credential_id}/grok-wake/remove\n  method: post\n  operationId: remove_grok_wake_v1_setup_credentials__credential_id__grok_wake_remove_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credentials/{credential_id}/rename\n  method: post\n  operationId: rename_installation_credential_v1_setup_credentials__credential_id__rename_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/billing-portal\n  method: post\n  operationId: billing_portal_v1_setup_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/upgrade\n  method: post\n  operationId:\
  \ upgrade_v1_setup_upgrade_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/credits\n  method: post\n  operationId: buy_credits_v1_setup_credits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: get\n  operationId: login_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/pin\n  method: post\n  operationId: login_with_pin_v1_auth_pin_post\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verification/start\n  method: post\n  operationId: start_login_verification_v1_auth_verification_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verification/check\n  method: post\n  operationId: check_login_verification_v1_auth_verification_check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/logout\n  method: post\n  operationId: logout_v1_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/stripe\n  method: post\n  operationId: stripe_webhook_v1_webhooks_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/public/sms-usage-options\n  method: get\n  operationId: sms_usage_options_v1_public_sms_usage_options_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credential\n  method: get\n  operationId: credential_status_v1_credential_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/installations/connected\n  method: post\n  operationId: installation_connected_v1_installations_connected_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bridges\n  method: post\n  operationId: open_bridge_v1_bridges_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bridges/{bridge_id}\n  method: get\n  operationId: get_bridge_v1_bridges__bridge_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bridges/{bridge_id}/close\n  method: post\n  operationId: close_bridge_v1_bridges__bridge_id__close_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bridges/{bridge_id}/messages\n  method: get\n  operationId: check_bridge_messages_v1_bridges__bridge_id__messages_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bridges/{bridge_id}/ack\n  method: post\n  operationId: acknowledge_bridge_messages_v1_bridges__bridge_id__ack_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bridges/{bridge_id}/messages/send\n  method: post\n  operationId: send_bridge_message_v1_bridges__bridge_id__messages_send_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/webhooks/sms/inbound\n  method: post\n  operationId: inbound_sms_v1_webhooks_sms_inbound_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setup/review-reply\n  method: post\n  operationId: review_reply_v1_setup_review_reply_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/campfiresms-com/agentic-access/campfiresms-com-agentic-access.yml
summary_line: 42 operations · 33 acting · 1 human-in-the-loop
tags:
- SMS
- Artificial Intelligence
- Automation
- Messaging
- Integration
---
