---
acting_count: 188
action_class_counts:
  acting: 188
  connected: 56
api_specs:
- filename: stytch-consumer-openapi.yml
  format: yaml
  label: Stytch Consumer Authentication API
  slug: stytch-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-consumer-openapi.yml
- filename: stytch-b2b-openapi.yml
  format: yaml
  label: Stytch B2B Authentication API
  slug: stytch-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-b2b-openapi.yml
- filename: stytch-management-openapi.yml
  format: yaml
  label: Stytch Management API
  slug: stytch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-management-openapi.yml
consequence_counts:
  physical: 7
  read: 56
  safety-critical: 18
  write: 163
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Stytch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pwa/v3/projects/:project_slug/environments/:environment_slug/event_log_streaming/:destination_type/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/organizations/{organization_id}/members/{member_id}/connected_apps/{connected_app_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/discovery/email/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/discovery/email/reset/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/email/require_reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/email/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/email/reset/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/existing_password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/passwords/session/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/b2b/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/magic_links/email/revoke_invite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/passwords/email/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/passwords/email/reset/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/passwords/existing_password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/passwords/session/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/users/{user_id}/connected_apps/{connected_app_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/verdict_reasons/override
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/b2b/magic_links/email/discovery/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/b2b/otps/email/discovery/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/b2b/otps/sms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/magic_links/email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/otps/email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/otps/sms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/otps/whatsapp/send
operation_count: 244
overview: 'Stytch exposes 244 API operations that an AI agent could call, of which 188 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 56 read, 163 write, 7 physical, and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stytch
provider_slug: stytch
slug: stytch-agentic-access
source_filename: stytch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/stytch-b2b-openapi.yml, openapi/stytch-consumer-openapi.yml, openapi/stytch-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 244\n  by_action_class:\n    acting: 188\n    connected: 56\n  by_consequence:\n    write: 163\n    read: 56\n    safety-critical: 18\n    physical: 7\n  human_in_the_loop_required: 18\noperations:\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}\n  method: put\n  operationId: api_b2b_scim_v1_b2b_scim_connection_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}\n  method: delete\n  operationId: api_b2b_scim_v1_b2b_scim_connection_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}\n  method: get\n  operationId: api_b2b_scim_v1_b2b_scim_connection_GetGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}/rotate/start\n  method: post\n  operationId: api_b2b_scim_v1_b2b_scim_connection_RotateStart\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}/rotate/complete\n  method: post\n  operationId: api_b2b_scim_v1_b2b_scim_connection_RotateComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection/{connection_id}/rotate/cancel\n  method: post\n  operationId: api_b2b_scim_v1_b2b_scim_connection_RotateCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection\n  method: post\n  operationId: api_b2b_scim_v1_b2b_scim_connection_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/scim/{organization_id}/connection\n  method: get\n  operationId: api_b2b_scim_v1_b2b_scim_connection_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations\n  method: post\n  operationId: api_organization_v1_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}\n  method: get\n  operationId: api_organization_v1_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}\n  method: put\n  operationId: api_organization_v1_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}\n  method: delete\n  operationId: api_organization_v1_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/search\n  method: post\n  operationId: api_organization_v1_Search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/metrics\n  method: get\n  operationId: api_organization_v1_Metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/connected_apps\n  method: get\n  operationId: api_organization_v1_ConnectedApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/connected_apps/{connected_app_id}\n  method: get\n  operationId: api_organization_v1_GetConnectedApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/external_id\n  method: delete\n  operationId: api_organization_v1_DeleteExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}\n  method: put\n  operationId: api_organization_v1_organizations_members_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}\n  method: delete\n  operationId: api_organization_v1_organizations_members_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/reactivate\n  method: put\n  operationId: api_organization_v1_organizations_members_Reactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/mfa_phone_numbers/{member_id}\n  method: delete\n  operationId: api_organization_v1_organizations_members_DeleteMFAPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/totp\n  method: delete\n  operationId: api_organization_v1_organizations_members_DeleteTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/members/search\n\
  \  method: post\n  operationId: api_organization_v1_organizations_members_Search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/passwords/{member_password_id}\n  method: delete\n  operationId: api_organization_v1_organizations_members_DeletePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/members/dangerously_get/{member_id}\n  method: get\n  operationId: api_organization_v1_organizations_members_DangerouslyGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oidc_providers\n  method: get\n  operationId: api_organization_v1_organizations_members_OIDCProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/unlink_retired_email\n  method: post\n  operationId: api_organization_v1_organizations_members_UnlinkRetiredEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/start_email_update\n  method: post\n  operationId:\
  \ api_organization_v1_organizations_members_StartEmailUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/connected_apps\n  method: get\n  operationId: api_organization_v1_organizations_members_GetConnectedApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/external_id\n  method: delete\n  operationId: api_organization_v1_organizations_members_DeleteExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/members\n  method: post\n  operationId: api_organization_v1_organizations_members_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/organizations/{organization_id}/member\n  method: get\n  operationId: api_organization_v1_organizations_members_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oauth_providers/google\n  method: get\n  operationId: api_organization_v1_organizations_members_oauth_providers_Google\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oauth_providers/microsoft\n  method: get\n  operationId: api_organization_v1_organizations_members_oauth_providers_Microsoft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oauth_providers/slack\n  method: get\n  operationId: api_organization_v1_organizations_members_oauth_providers_Slack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oauth_providers/hubspot\n  method: get\n  operationId: api_organization_v1_organizations_members_oauth_providers_Hubspot\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/oauth_providers/github\n  method: get\n  operationId: api_organization_v1_organizations_members_oauth_providers_Github\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/organizations/{organization_id}/members/{member_id}/connected_apps/{connected_app_id}/revoke\n  method: post\n  operationId: api_organization_v1_organizations_members_connected_apps_Revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/idp/oauth/authorize/start\n\
  \  method: post\n  operationId: api_b2b_idp_v1_b2b_idp_oauth_AuthorizeStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/idp/oauth/authorize\n  method: post\n  operationId: api_b2b_idp_v1_b2b_idp_oauth_Authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions\n  method: get\n  operationId: api_b2b_session_v1_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/sessions/authenticate\n\
  \  method: post\n  operationId: api_b2b_session_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions/revoke\n  method: post\n  operationId: api_b2b_session_v1_Revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/sessions/exchange\n  method: post\n  operationId: api_b2b_session_v1_Exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions/exchange_access_token\n  method: post\n  operationId: api_b2b_session_v1_ExchangeAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions/attest\n  method: post\n  operationId: api_b2b_session_v1_Attest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions/migrate\n  method: post\n  operationId: api_b2b_session_v1_Migrate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sessions/jwks/{project_id}\n  method: get\n  operationId: api_b2b_session_v1_GetJWKS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/impersonation/authenticate\n  method: post\n  operationId: api_b2b_impersonation_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/rbac/policy\n  method: get\n  operationId: api_b2b_rbac_v1_Policy\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/rbac/organizations/{organization_id}\n  method: get\n  operationId: api_b2b_rbac_v1_b2b_rbac_organizations_GetOrgPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/rbac/organizations/{organization_id}\n  method: put\n  operationId: api_b2b_rbac_v1_b2b_rbac_organizations_SetOrgPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/recovery_codes/recover\n  method: post\n  operationId: api_b2b_recovery_codes_v1_Recover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/recovery_codes/{organization_id}/{member_id}\n  method: get\n  operationId: api_b2b_recovery_codes_v1_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/recovery_codes/rotate\n  method: post\n  operationId: api_b2b_recovery_codes_v1_Rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/totp\n  method: post\n  operationId: api_b2b_totp_v1_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/totp/authenticate\n  method: post\n  operationId: api_b2b_totp_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/totp/migrate\n  method: post\n  operationId: api_b2b_totp_v1_Migrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/discovery/intermediate_sessions/exchange\n  method: post\n  operationId:\
  \ api_discovery_v1_discovery_intermediate_sessions_Exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/discovery/organizations/create\n  method: post\n  operationId: api_discovery_v1_discovery_organizations_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/discovery/organizations\n  method: post\n  operationId: api_discovery_v1_discovery_organizations_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/magic_links/authenticate\n  method: post\n  operationId: api_b2b_magic_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/magic_links/email/login_or_signup\n  method: post\n  operationId: api_b2b_magic_v1_b2b_magic_links_email_LoginOrSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/magic_links/email/invite\n  method: post\n  operationId:\
  \ api_b2b_magic_v1_b2b_magic_links_email_Invite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/magic_links/email/discovery/send\n  method: post\n  operationId: api_b2b_magic_v1_b2b_magic_links_email_discovery_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/magic_links/discovery/authenticate\n  method: post\n  operationId: api_b2b_magic_v1_b2b_magic_links_discovery_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/oauth/authenticate\n  method: post\n  operationId: api_b2b_oauth_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/oauth/discovery/authenticate\n  method: post\n  operationId: api_b2b_oauth_v1_b2b_oauth_discovery_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/otps/sms/send\n\
  \  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_sms_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/otps/sms/authenticate\n  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_sms_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/otps/email/login_or_signup\n  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_email_LoginOrSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/otps/email/authenticate\n  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_email_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/otps/email/discovery/send\n  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_email_discovery_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/b2b/otps/email/discovery/authenticate\n  method: post\n  operationId: api_b2b_otp_v1_b2b_otp_email_discovery_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/passwords/strength_check\n  method: post\n  operationId: api_b2b_password_v1_StrengthCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/passwords/migrate\n  method: post\n  operationId: api_b2b_password_v1_Migrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/passwords/authenticate\n  method: post\n  operationId: api_b2b_password_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/passwords/email/reset/start\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_email_ResetStart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/b2b/passwords/email/reset\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_email_Reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/passwords/email/require_reset\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_email_RequireReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/passwords/session/reset\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_session_Reset\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/passwords/existing_password/reset\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_existing_password_Reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/passwords/discovery/authenticate\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_discovery_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/passwords/discovery/email/reset/start\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_discovery_email_ResetStart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/passwords/discovery/email/reset\n  method: post\n  operationId: api_b2b_password_v1_b2b_passwords_discovery_email_Reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/b2b/sso/{organization_id}\n  method: get\n  operationId: api_sso_v1_GetConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/b2b/sso/{organization_id}/connections/{connection_id}\n  method: delete\n  operationId: api_sso_v1_DeleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/b2b/sso/authenticate\n  method: post\n  operationId: api_sso_v1_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    \n\n# --- truncated at 32 KB (86 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/agentic-access/stytch-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/agentic-access/stytch-agentic-access.yml
summary_line: 244 operations · 188 acting · 18 human-in-the-loop
tags:
- Authentication
- Identity
- Passwordless
- Security
- B2B
- Connected Apps
- MCP
- AI Agents
- Developer Tools
---
