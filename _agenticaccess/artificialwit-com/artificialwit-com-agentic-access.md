---
acting_count: 59
action_class_counts:
  acting: 59
  connected: 27
api_specs:
- filename: artificialwit-com-ai-agent-api-api-openapi.yml
  format: yaml
  label: Artificial Wit AI Agent API
  slug: artificialwit-com-ai-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-ai-agent-api-api-openapi.yml
- filename: artificialwit-com-auth-api-openapi.yml
  format: yaml
  label: Artificial Wit Auth API
  slug: artificialwit-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-auth-api-openapi.yml
- filename: artificialwit-com-chat-api-openapi.yml
  format: yaml
  label: Artificial Wit Chat API
  slug: artificialwit-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-chat-api-openapi.yml
- filename: artificialwit-com-embed-api-openapi.yml
  format: yaml
  label: Artificial Wit Embed API
  slug: artificialwit-com-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-embed-api-openapi.yml
- filename: artificialwit-com-file-api-openapi.yml
  format: yaml
  label: Artificial Wit File API
  slug: artificialwit-com-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-file-api-openapi.yml
- filename: artificialwit-com-hub-api-openapi.yml
  format: yaml
  label: Artificial Wit Hub API
  slug: artificialwit-com-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-hub-api-openapi.yml
- filename: artificialwit-com-mcp-api-openapi.yml
  format: yaml
  label: Artificial Wit MCP API
  slug: artificialwit-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-mcp-api-openapi.yml
- filename: artificialwit-com-mcp-oauth-api-openapi.yml
  format: yaml
  label: Artificial Wit MCP OAUTH API
  slug: artificialwit-com-mcp-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-mcp-oauth-api-openapi.yml
- filename: artificialwit-com-members-api-openapi.yml
  format: yaml
  label: Artificial Wit Members API
  slug: artificialwit-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-members-api-openapi.yml
- filename: artificialwit-com-messaging-api-openapi.yml
  format: yaml
  label: Artificial Wit Messaging API
  slug: artificialwit-com-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-messaging-api-openapi.yml
- filename: artificialwit-com-meta-api-openapi.yml
  format: yaml
  label: Artificial Wit Meta API
  slug: artificialwit-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-meta-api-openapi.yml
- filename: artificialwit-com-payment-api-openapi.yml
  format: yaml
  label: Artificial Wit Payment API
  slug: artificialwit-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-payment-api-openapi.yml
- filename: artificialwit-com-rest-api-openapi.yml
  format: yaml
  label: Artificial Wit Rest API
  slug: artificialwit-com-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-rest-api-openapi.yml
- filename: artificialwit-com-scim-api-openapi.yml
  format: yaml
  label: Artificial Wit SCIM API
  slug: artificialwit-com-scim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-scim-api-openapi.yml
- filename: artificialwit-com-template-api-openapi.yml
  format: yaml
  label: Artificial Wit Template API
  slug: artificialwit-com-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-template-api-openapi.yml
- filename: artificialwit-com-things-api-openapi.yml
  format: yaml
  label: Artificial Wit Things API
  slug: artificialwit-com-things-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-things-api-openapi.yml
- filename: artificialwit-com-website-api-openapi.yml
  format: yaml
  label: Artificial Wit Website API
  slug: artificialwit-com-website-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artificialwit-com/openapi/artificialwit-com-website-api-openapi.yml
consequence_counts:
  physical: 10
  read: 27
  safety-critical: 1
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Artificialwit Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset_password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hub/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /members/resend-invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/conversations/{conversation_id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/checkout/stripe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/confirm/stripe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/order/razorpay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/subscription/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/verify/razorpay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/webhook/razorpay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/webhook/stripe
operation_count: 86
overview: 'Artificial Wit exposes 86 API operations that an AI agent could call, of which 59 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 48 write, 10 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Artificial Wit
provider_slug: artificialwit-com
slug: artificialwit-com-agentic-access
source_filename: artificialwit-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/artificialwit-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 86\n  by_action_class:\n    acting: 59\n    connected: 27\n  by_consequence:\n    physical: 10\n    write: 48\n    safety-critical: 1\n    read: 27\n  human_in_the_loop_required: 1\noperations:\n- path: /hub/send\n  method: post\n  operationId: hub_send_hub_send_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat\n\
  \  method: post\n  operationId: chat_chat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed\n  method: post\n  operationId: embed_embed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token\n  method: post\n  operationId: token_auth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /auth/refresh_token\n  method: post\n  operationId: refresh_token_auth_refresh_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/forgot_password\n  method: post\n  operationId: forgot_password_auth_forgot_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/reset_password\n  method: post\n  operationId: reset_password_auth_reset_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/users\n  method: post\n  operationId: create_user_auth_users_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/change_password\n  method: post\n  operationId: change_password_auth_change_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/saml/init\n  method: get\n  operationId: saml_init_auth_saml_init_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/saml/acs\n  method: post\n  operationId: saml_acs_auth_saml_acs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/saml/verify\n  method: post\n  operationId: saml_verify_auth_saml_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/mobile/otp/request\n  method: post\n  operationId: mobile_otp_request_auth_mobile_otp_request_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/mobile/otp/verify\n  method: post\n  operationId: mobile_otp_verify_auth_mobile_otp_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/mfa/login\n  method: post\n  operationId: mfa_login_auth_mfa_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /mcp/\n  method: get\n  operationId: sse_connect_mcp__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/\n  method: post\n  operationId: handle_message_mcp__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/artifacts\n  method: get\n  operationId: list_artifacts_mcp_artifacts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/artifacts/{filename}\n  method: get\n  operationId: get_artifact_mcp_artifacts__filename__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: oauth_protected_resource__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: oauth_authorization_server__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/register\n  method: post\n  operationId: oauth_register_oauth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /oauth/authorize\n  method: get\n  operationId: oauth_authorize_oauth_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize-submit\n  method: post\n  operationId: oauth_authorize_submit_oauth_authorize_submit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize-submit-credentials\n  method: post\n  operationId: oauth_authorize_submit_credentials_oauth_authorize_submit_credentials_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: oauth_token_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/upload/{bucket}\n  method: post\n  operationId: upload_file_file_upload__bucket__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/upload\n  method: post\n  operationId: upload_file_file_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/download/{bucket}\n  method: post\n  operationId: download_file_file_download__bucket__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/download\n  method: post\n  operationId: download_file_file_download_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/{stored_filename}\n  method: delete\n  operationId: delete_file_file__stored_filename__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/direct\n  method: post\n  operationId: create_direct_conversation_messaging_conversations_direct_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/group\n  method: post\n  operationId: create_group_conversation_messaging_conversations_group_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations\n  method: get\n  operationId: list_conversations_messaging_conversations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/conversations/{conversation_id}\n  method: get\n  operationId: get_conversation_messaging_conversations__conversation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/conversations/{conversation_id}\n  method: patch\n  operationId: update_group_conversation_messaging_conversations__conversation_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/archive\n  method: post\n  operationId: archive_conversation_messaging_conversations__conversation_id__archive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/leave\n  method: post\n  operationId: leave_conversation_messaging_conversations__conversation_id__leave_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/participants\n\
  \  method: post\n  operationId: add_participants_messaging_conversations__conversation_id__participants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/participants/{profile_id}\n  method: delete\n  operationId: remove_participant_messaging_conversations__conversation_id__participants__profile_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/participants/{profile_id}/role\n  method: patch\n  operationId: update_participant_role_messaging_conversations__conversation_id__participants__profile_id__role_patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/messages\n  method: post\n  operationId: send_message_messaging_conversations__conversation_id__messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/messages\n  method: get\n  operationId: list_messages_messaging_conversations__conversation_id__messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/messages/{message_id}\n  method: patch\n  operationId: edit_message_messaging_messages__message_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/messages/{message_id}\n  method: delete\n  operationId: delete_message_messaging_messages__message_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/conversations/{conversation_id}/read\n  method: post\n  operationId: mark_conversation_read_messaging_conversations__conversation_id__read_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/unread-counts\n  method: get\n  operationId: get_unread_counts_messaging_unread_counts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/search\n  method: get\n  operationId: search_messages_messaging_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/file/{bucket}/{object_path}\n  method: get\n  operationId: download_public_file_rest_public_file__bucket___object_path__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/{fn_name}\n  method: post\n  operationId: call_rpc_public_rest_public__fn_name__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/{fn_name}\n  method: post\n  operationId: call_rpc_rest__fn_name__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/ServiceProviderConfig\n  method: get\n  operationId: service_provider_config_scim_v2_ServiceProviderConfig_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: get\n  operationId: list_users_scim_v2_Users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: post\n  operationId: create_user_scim_v2_Users_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: get\n  operationId: get_user_scim_v2_Users__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users/{user_id}\n  method: put\n  operationId: replace_user_scim_v2_Users__user_id__put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: patch\n  operationId: patch_user_scim_v2_Users__user_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: delete\n  operationId: delete_user_scim_v2_Users__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups\n  method: get\n  operationId: list_groups_scim_v2_Groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Groups\n  method: post\n  operationId: create_group_scim_v2_Groups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: get\n  operationId: get_group_scim_v2_Groups__group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Groups/{group_id}\n  method: put\n  operationId: replace_group_scim_v2_Groups__group_id__put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: patch\n  operationId: patch_group_scim_v2_Groups__group_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: delete\n  operationId: delete_group_scim_v2_Groups__group_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /things/{protocol}/{x_api_key}\n  method: post\n  operationId: receive_thing_data_things__protocol___x_api_key__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /things/{protocol}/{x_api_key}\n  method: get\n  operationId: receive_thing_data_things__protocol___x_api_key__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /website/contact\n  method: post\n  operationId: contact_website_contact_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /website/signup\n  method: post\n  operationId: signup_website_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/invite\n  method: post\n  operationId: invite_member_members_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/resend-invite\n  method: post\n  operationId: resend_invite_members_resend_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/{format}\n  method: post\n  operationId: render_from_body_template__format__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/{route_name}/{data_id}/{format}/{template_id}/{language_id}\n  method: get\n  operationId: render_from_db_template__route_name___data_id___format___template_id___language_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template/{route_name}/{data_id}/{format}/{template_id}\n\
  \  method: get\n  operationId: render_from_db_template__route_name___data_id___format___template_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/plans\n  method: get\n  operationId: get_plans_payment_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/checkout/stripe\n  method: post\n  operationId: create_stripe_checkout_payment_checkout_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/order/razorpay\n  method: post\n  operationId: create_razorpay_order_payment_order_razorpay_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/verify/razorpay\n  method: post\n  operationId: verify_razorpay_payment_payment_verify_razorpay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/confirm/stripe\n  method: post\n  operationId: confirm_stripe_session_payment_confirm_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/subscription\n  method: get\n  operationId: get_subscription_payment_subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/subscription/cancel\n  method: post\n  operationId: cancel_subscription_payment_subscription_cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/transactions\n  method: get\n  operationId:\
  \ get_transactions_payment_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/admin/subscriptions\n  method: get\n  operationId: get_all_subscriptions_payment_admin_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/webhook/stripe\n  method: post\n  operationId: stripe_webhook_payment_webhook_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/webhook/razorpay\n  method: post\n  operationId: razorpay_webhook_payment_webhook_razorpay_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/artificialwit-com/agentic-access/artificialwit-com-agentic-access.yml
summary_line: 86 operations · 59 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Enterprise
- Legacy Systems
- MCP
- Integration
---
