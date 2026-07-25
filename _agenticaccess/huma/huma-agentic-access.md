---
acting_count: 527
action_class_counts:
  acting: 527
  connected: 457
api_specs:
- filename: huma-platform-openapi-original.yml
  format: yaml
  label: Huma Integration API
  slug: huma-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/openapi/huma-platform-openapi-original.yml
consequence_counts:
  physical: 124
  read: 457
  safety-critical: 6
  write: 397
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Huma Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/v1/password-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/v1/request-password-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extensions/v1/admin/deployment/{deployment_id}/reset-demo-user
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extensions/v1/deployment/clone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extensions/v1/user/{user_id}/module-result/AsthmaControlTest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extensions/v1/user/{user_id}/module-result/AsthmaControlTest/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/v1/sendverificationtoken
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/template-bank/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/template-bank/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/admin/send-invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/create-patient-profile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/file-library
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/full
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/extensions/v1/deployment/invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/invitation-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/extensions/v1/deployment/invitation/{invitation_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/move
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/resend-invitation-list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/send-invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/send-invitation/{user_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/extensions/v1/deployment/template
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/extensions/v1/deployment/template/{template_id}
operation_count: 984
overview: 'Huma exposes 984 API operations that an AI agent could call, of which 527 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 457 read, 397 write, 124 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Huma
provider_slug: huma
slug: huma-agentic-access
source_filename: huma-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/huma-platform-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 984\n  by_action_class:\n    connected: 457\n    acting: 527\n  by_consequence:\n    read: 457\n    write: 397\n    safety-critical: 6\n    physical: 124\n  human_in_the_loop_required: 6\noperations:\n- path: /.well-known/apple-app-site-association\n  method: get\n  operationId: .well_known_apple_app_site_association_retrieve_[retrieve_deeplink_for_apple_app]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/assetlinks.json\n  method: get\n  operationId: .well_known_assetlinks.json_retrieve_[retrieve_deeplink_for_android_app]\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/v1/authprofile\n  method: post\n  operationId: api_auth_v1_authprofile_create_[auth_profile]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/check-auth-attributes\n  method: post\n  operationId: api_auth_v1_check_auth_attributes_create_[check_auth_attributes]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/confirm\n  method: post\n\
  \  operationId: api_auth_v1_confirm_create_[confirmation]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/me\n  method: get\n  operationId: api_auth_v1_me_retrieve_[me]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/v1/password-reset\n  method: post\n  operationId: api_auth_v1_password_reset_create_[password_reset]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/auth/v1/private/user/{user_id}/delete-user\n  method: delete\n  operationId: api_auth_v1_private_user_delete_user_destroy_[delete_user]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/refreshtoken\n  method: post\n  operationId: api_auth_v1_refreshtoken_create_[refresh_token_v1]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/request-code\n  method: post\n  operationId: api_auth_v1_request_code_create_[request_code]\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/request-password-reset\n  method: post\n  operationId: api_auth_v1_request_password_reset_create_[request_password_reset]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/v1/sendverificationtoken\n  method: post\n  operationId: api_auth_v1_sendverificationtoken_create_[send_verification_token]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/service-account\n  method: post\n  operationId: api_auth_v1_service_account_create_[create_service_account]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/set-auth-attributes\n  method: post\n  operationId: api_auth_v1_set_auth_attributes_create_[set_auth_attributes]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/signin\n  method: post\n\
  \  operationId: api_auth_v1_signin_create_[sign_in_v1]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/signout\n  method: post\n  operationId: api_auth_v1_signout_create_[sign_out_v1]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/signup\n  method: post\n  operationId: api_auth_v1_signup_create_[sign_up]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/sso/callback\n  method: post\n  operationId: api_auth_v1_sso_callback_create_[saml_callback]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/sso/oidc-callback\n  method: get\n  operationId: api_auth_v1_sso_oidc_callback_retrieve_[oidc_callback]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/v1/sso/request\n  method: post\n  operationId: api_auth_v1_sso_request_create_[sso_request]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/user/{user_id}/api-key\n  method: get\n  operationId: api_auth_v1_user_api_key_retrieve_[retrieve_api_keys]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/v1/user/{user_id}/api-key\n  method: post\n  operationId: api_auth_v1_user_api_key_create_[generate_api_key]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/user/{user_id}/api-key/{key_id}\n  method: delete\n  operationId: api_auth_v1_user_api_key_destroy_[delete_api_key]\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/user/{user_id}/sessions\n  method: get\n  operationId: api_auth_v1_user_sessions_retrieve_[retrieve_sessions]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/v1/user/{user_id}/token\n  method: post\n  operationId: api_auth_v1_user_token_create_[generate_auth_token]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/v1/verify\n  method: post\n  operationId: api_auth_v1_verify_create_[verify_credentials]\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/autocomplete/v1/AZVaccineBatchNumber/search\n  method: get\n  operationId: api_autocomplete_v1_AZVaccineBatchNumber_search_retrieve_[func]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete/v1/Indications/search\n  method: get\n  operationId: api_autocomplete_v1_Indications_search_retrieve_[func]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete/v1/Medications/search\n  method: get\n  operationId: api_autocomplete_v1_Medications_search_retrieve_[func]\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete/v1/MedicationsV2/search\n  method: get\n  operationId: api_autocomplete_v1_MedicationsV2_search_retrieve_[func]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete/v1/Symptoms/search\n  method: get\n  operationId: api_autocomplete_v1_Symptoms_search_retrieve_[func]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete/v1/update\n  method: post\n  operationId: api_autocomplete_v1_update_create_[update_autocomplete_metadata]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calendar/v1/render/test\n  method: get\n  operationId: api_calendar_v1_render_test_retrieve_[test_calendar]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar/v1/user/{user_id}/export\n  method: get\n  operationId: api_calendar_v1_user_export_retrieve_[export_calendar]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/care-plan/v1/user/{user_id}/care-plan\n  method: get\n  operationId: api_care_plan_v1_user_care_plan_retrieve_[retrieve_care_plan]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/care-plan/v1/user/{user_id}/care-plan\n  method: post\n \
  \ operationId: api_care_plan_v1_user_care_plan_create_[assign_care_plan]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/care-plan/v1/user/{user_id}/cycler/mock\n  method: post\n  operationId: api_care_plan_v1_user_cycler_mock_create_[mock_adp_cycler_data]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/care-plan/v1/user/{user_id}/prescription\n  method: post\n  operationId: api_care_plan_v1_user_prescription_create_[create_prescription]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/care-plan/v1/user/{user_id}/prescriptions\n  method: get\n  operationId: api_care_plan_v1_user_prescriptions_retrieve_[retrieve_prescriptions]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cds/v1/user/{user_id}/pregnancy\n  method: post\n  operationId: api_cds_v1_user_pregnancy_create_[update_pregnancy_info]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/firmware-bank/archive\n  method: post\n  operationId:\
  \ api_extensions_firmware_bank_archive_create_[archive_firmware]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/firmware-bank/list\n  method: get\n  operationId: api_extensions_firmware_bank_list_retrieve_[retrieve_firmware_updates]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/firmware-bank/upload\n  method: post\n  operationId: api_extensions_firmware_bank_upload_create_[upload_firmware]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/template-bank/create\n  method: post\n  operationId: api_extensions_template_bank_create_create_[shared_templates_bank_create]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/template-bank/import\n  method: post\n  operationId: api_extensions_template_bank_import_create_[import_template_deployment_config]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/template-bank/list\n\
  \  method: get\n  operationId: api_extensions_template_bank_list_retrieve_[shared_templates_bank_list]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/template-bank/remove\n  method: post\n  operationId: api_extensions_template_bank_remove_create_[remove_template_deployment_config]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/admin/deployment/{deployment_id}/demo-url\n  method: get\n  operationId: api_extensions_v1_admin_deployment_demo_url_retrieve_[get_demo_user_url]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/admin/deployment/{deployment_id}/reset-demo-user\n  method: post\n  operationId: api_extensions_v1_admin_deployment_reset_demo_user_create_[reset_demo_user_url]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/extensions/v1/admin/invites\n  method: get\n  operationId: api_extensions_v1_admin_invites_retrieve_[retrieve_invites]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/admin/invites\n  method: post\n  operationId: api_extensions_v1_admin_invites_create_[invite]\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/admin/send-invitation\n  method: post\n  operationId: api_extensions_v1_admin_send_invitation_create_[send_admin_invitations]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/admin/service-account\n  method: post\n  operationId: api_extensions_v1_admin_service_account_create_[generate_service_account_api_key]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/admin/service-account\n  method: delete\n  operationId: api_extensions_v1_admin_service_account_destroy_[delete_user_service_account]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/admin/staff\n  method: get\n  operationId: api_extensions_v1_admin_staff_retrieve_[search_staff]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/assets\n  method: post\n  operationId: api_extensions_v1_assets_create_[create_content]\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/assets/{content_id}\n  method: get\n  operationId: api_extensions_v1_assets_retrieve_[retrieve_content]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/assets/{content_id}\n  method: put\n  operationId: api_extensions_v1_assets_update_[update_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/assets/{content_id}\n  method: delete\n\
  \  operationId: api_extensions_v1_assets_destroy_[delete_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/assets/schema\n  method: get\n  operationId: api_extensions_v1_assets_schema_retrieve_[retrieve_schema]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/assets/search\n  method: post\n  operationId: api_extensions_v1_assets_search_create_[search_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/extensions/v1/billing/log-actions\n  method: get\n  operationId: api_extensions_v1_billing_log_actions_retrieve_[retrieve_billing_monitoring_log_action_list]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/billing/profiles\n  method: post\n  operationId: api_extensions_v1_billing_profiles_create_[retrieve_billing_alerts]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}\n  method: get\n  operationId: api_extensions_v1_billing_user_retrieve_[calculate_cumulative_monitoring_time_and_cpt_code]\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/billing/user/{user_id}\n  method: post\n  operationId: api_extensions_v1_billing_user_create_[create_billing_remote_time_tracking]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}/log\n  method: post\n  operationId: api_extensions_v1_billing_user_log_create_[create_billing_monitoring_log]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}/log/{log_id}\n\
  \  method: put\n  operationId: api_extensions_v1_billing_user_log_update_[update_billing_monitoring_log]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}/log/{log_id}\n  method: delete\n  operationId: api_extensions_v1_billing_user_log_destroy_[delete_billing_monitoring_log]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}/logs\n  method: post\n  operationId: api_extensions_v1_billing_user_logs_create_[retrieve_billing_monitoring_logs]\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/billing/user/{user_id}/report\n  method: get\n  operationId: api_extensions_v1_billing_user_report_retrieve_[report_billing_records_for_cpt]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/cms/{collection}\n  method: post\n  operationId: api_extensions_v1_cms_create_[create_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/extensions/v1/cms/{collection}/{content_id}\n  method: get\n  operationId: api_extensions_v1_cms_retrieve_[retrieve_content]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/cms/{collection}/{content_id}\n  method: put\n  operationId: api_extensions_v1_cms_update_[update_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/cms/{collection}/{content_id}\n  method: delete\n  operationId: api_extensions_v1_cms_destroy_[delete_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/cms/{collection}/{content_id}/{version}\n  method: get\n  operationId: api_extensions_v1_cms_retrieve_[retrieve_content_version]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/cms/{collection}/{content_id}/publish\n  method: post\n  operationId: api_extensions_v1_cms_publish_create_[publish_draft]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/cms/{collection}/schema\n  method: get\n  operationId: api_extensions_v1_cms_schema_retrieve_[retrieve_schema]\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/cms/{collection}/search\n  method: post\n  operationId: api_extensions_v1_cms_search_create_[search_content]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/cms/{collection}/tags\n  method: get\n  operationId: api_extensions_v1_cms_tags_retrieve_[retrieve_collection_tags]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/cms/collections\n  method: get\n  operationId: api_extensions_v1_cms_collections_retrieve_[list_collections]\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/dashboards/{resource_type}/{resource_id}\n  method: get\n  operationId: api_extensions_v1_dashboards_retrieve_[retrieve_dashboards]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/dashboards/{resource_type}/{resource_id}/dashboard/{dashboard_id}\n  method: get\n  operationId: api_extensions_v1_dashboards_dashboard_retrieve_[retrieve_dashboard]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/dashboards/{resource_type}/{resource_id}/gadget/{gadget_id}/data\n  method: post\n  operationId: api_extensions_v1_dashboards_gadget_data_create_[retrieve_gadget_data]\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/dashboards/data\n  method: post\n  operationId: api_extensions_v1_dashboards_data_create_[multi_resource_dashboard_data]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/dashboards/deployment/{deployment_id}/stats\n  method: get\n  operationId: api_extensions_v1_dashboards_deployment_stats_retrieve_[retrieve_deployment_stats]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/deployment\n\
  \  method: post\n  operationId: api_extensions_v1_deployment_create_[create_deployment]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/deployment/{deployment_id}\n  method: get\n  operationId: api_extensions_v1_deployment_retrieve_[retrieve_deployment]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/v1/deployment/{deployment_id}\n  method: put\n  operationId: api_extensions_v1_deployment_update_[update_deployment]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/deployment/{deployment_id}/component-config\n  method: post\n  operationId: api_extensions_v1_deployment_component_config_create_[create_component_config]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/v1/deployment/{deployment_id}/component-config\n  method: put\n  operationId: api_extensions_v1_deployment_component_config_update_[update_\n\n# --- truncated at 32 KB (373 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/agentic-access/huma-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/agentic-access/huma-agentic-access.yml
summary_line: 984 operations · 527 acting · 6 human-in-the-loop
tags:
- Healthcare
- United Kingdom
- Remote Patient Monitoring
- Telehealth
- Digital Health
- Clinical Trials
- SDK
- Medical Device Software
- Population Health
---
