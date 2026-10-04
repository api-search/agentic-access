---
acting_count: 350
action_class_counts:
  acting: 350
  connected: 109
api_specs:
- filename: descope-apps-api-openapi.yml
  format: yaml
  label: Descope Apps API
  slug: descope-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-apps-api-openapi.yml
- filename: descope-auth-api-openapi.yml
  format: yaml
  label: Descope Auth API
  slug: descope-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-auth-api-openapi.yml
- filename: descope-custom-attributes-api-openapi.yml
  format: yaml
  label: Descope Custom Attributes API
  slug: descope-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-custom-attributes-api-openapi.yml
- filename: descope-email-api-openapi.yml
  format: yaml
  label: Descope Email API
  slug: descope-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-email-api-openapi.yml
- filename: descope-embedded-link-api-openapi.yml
  format: yaml
  label: Descope Embedded Link API
  slug: descope-embedded-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-embedded-link-api-openapi.yml
- filename: descope-fedcm-api-openapi.yml
  format: yaml
  label: Descope Fedcm API
  slug: descope-fedcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-fedcm-api-openapi.yml
- filename: descope-instant-message-im-api-openapi.yml
  format: yaml
  label: Descope Instant Message (IM) API
  slug: descope-instant-message-im-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-instant-message-im-api-openapi.yml
- filename: descope-keys-api-openapi.yml
  format: yaml
  label: Descope Keys API
  slug: descope-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-keys-api-openapi.yml
- filename: descope-mgmt-api-openapi.yml
  format: yaml
  label: Descope Mgmt API
  slug: descope-mgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-mgmt-api-openapi.yml
- filename: descope-scim-api-openapi.yml
  format: yaml
  label: Descope Scim API
  slug: descope-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-scim-api-openapi.yml
- filename: descope-text-message-sms-api-openapi.yml
  format: yaml
  label: Descope Text Message (SMS) API
  slug: descope-text-message-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-text-message-sms-api-openapi.yml
- filename: descope-verification-api-openapi.yml
  format: yaml
  label: Descope Verification API
  slug: descope-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-verification-api-openapi.yml
- filename: descope-voice-message-phone-api-openapi.yml
  format: yaml
  label: Descope Voice Message (Phone) API
  slug: descope-voice-message-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-voice-message-phone-api-openapi.yml
- filename: descope-well-known-api-openapi.yml
  format: yaml
  label: Descope .well Known API
  slug: descope-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-well-known-api-openapi.yml
- filename: descope-oauth2-api-openapi.yml
  format: yaml
  label: Descope Oauth2 API
  slug: descope-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-oauth2-api-openapi.yml
consequence_counts:
  physical: 1
  read: 109
  safety-critical: 8
  write: 341
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Descope Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/v1/apps/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/v1/apps/{project_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/v1/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mgmt/outbound/app/create/bydcrpreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mgmt/stop/impersonation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mgmt/tenant/adminlinks/sso/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{ssoAppId}/oauth2/v1/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/mgmt/tenant/adminlinks/sso/send
operation_count: 459
overview: 'Descope exposes 459 API operations that an AI agent could call, of which 350 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 109 read, 341 write, 1 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Descope
provider_slug: descope
slug: descope-agentic-access
source_filename: descope-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/descope-apps-api-openapi.yml, openapi/descope-auth-api-openapi.yml, openapi/descope-custom-attributes-api-openapi.yml,\n  openapi/descope-default-api-openapi.yml, openapi/descope-email-api-openapi.yml, openapi/descope-embedded-link-api-openapi.yml,\n  openapi/descope-fedcm-api-openapi.yml, openapi/descope-instant-message-im-api-openapi.yml,\n  openapi/descope-keys-api-openapi.yml, openapi/descope-mgmt-api-openapi.yml, openapi/descope-oauth2-api-openapi.yml,\n  openapi/descope-scim-api-openapi.yml, openapi/descope-text-message-sms-api-openapi.yml, openapi/descope-verification-api-openapi.yml,\n  openapi/descope-voice-message-phone-api-openapi.yml, openapi/descope-well-known-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 459\n  by_action_class:\n    connected: 109\n    acting: 350\n  by_consequence:\n    read: 109\n    write: 341\n    safety-critical: 8\n    physical: 1\n  human_in_the_loop_required: 8\noperations:\n- path: /v1/apps/agentic/{projectId}/{mcpServerId}/.well-known/oauth-authorization-server\n  method: get\n  operationId: GetAgenticThirdPartyAppsWellKnownConfigurationAuthServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/agentic/{projectId}/{mcpServerId}/.well-known/openid-configuration\n  method: get\n  operationId: GetAgenticThirdPartyAppsWellKnownConfigurationOpenID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{projectId}/.well-known/oauth-authorization-server\n  method: get\n  operationId: GetThirdPartyAppsWellKnownConfigurationAuthServer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{projectId}/.well-known/openid-configuration\n  method: get\n  operationId: GetThirdPartyAppsWellKnownConfigurationOpenID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/saml/idp/initiate\n  method: get\n  operationId: SAMLIDPInitiateHTTPRedirectBinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/saml/idp/initiate\n  method: post\n  operationId: SAMLIDPInitiateHTTPPostBinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/saml/idp/sso\n  method: get\n  operationId: SAMLIDPHTTPRedirectBinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/saml/idp/sso\n  method: post\n  operationId: SAMLIDPHTTPPostBinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/saml/idp/sso-finish\n  method: post\n  operationId: SAMLIDPFinishEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auth/wsfed/idp/initiate\n  method: get\n  operationId: WSFedIDPInitiateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/wsfed/idp/initiate\n  method: post\n  operationId: WSFedIDPInitiatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/wsfed/idp/sso\n  method: get\n  operationId: WSFedIDPPassiveGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/wsfed/idp/sso\n  method: post\n  operationId: WSFedIDPPassivePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/wsfed/idp/sso-finish\n  method: post\n  operationId: WSFedIDPFinishEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/accesskey/exchange\n  method: post\n  operationId: ExchangeAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/refresh\n  method: post\n  operationId: RefreshSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/try-refresh\n  method: post\n  operationId: TryRefreshSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/me\n  method: get\n  operationId: Me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/me/history\n  method: get\n  operationId: MeAuthHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/tenant/select\n  method: post\n  operationId: SelectTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/idp/sso/logout\n  method: get\n  operationId: IDPSSOLogoutGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/idp/sso/logout\n  method: post\n  operationId: IDPSSOLogoutPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/logout\n\
  \  method: post\n  operationId: Logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/logoutall\n  method: post\n  operationId: LogoutAllDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/validate\n  method: post\n  operationId: ValidateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auth/notp/{provider}/update\n  method: post\n  operationId: UpdateUserNOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/authorize\n  method: post\n  operationId: AuthorizeOAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/authorize/signin\n  method: post\n  operationId: CreateOAuthRedirectURISignin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/authorize/signup\n  method: post\n  operationId: CreateOAuthRedirectURISignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/authorize/update\n  method: post\n  operationId: CreateOAuthRedirectURIUpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/native/start\n  method: post\n  operationId: OAuthNativeStart\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/exchange\n  method: post\n  operationId: ExchangeCodeoauth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/native/finish\n  method: post\n  operationId: OAuthNativeFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/onetap/idtoken/exchange\n\
  \  method: post\n  operationId: ExchangeOneTapIDToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/onetap/idtoken/verify\n  method: post\n  operationId: VerifyOneTapIDToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/onetap/clientid/{provider}\n  method: get\n  operationId: GetOneTapClientID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/password/signup\n  method: post\n  operationId:\
  \ SignUpPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/password/signin\n  method: post\n  operationId: SignInPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/password/replace\n  method: post\n  operationId: ReplaceUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v1/auth/password/update\n  method: post\n  operationId: UpdateUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/password/policy\n  method: get\n  operationId: GetPasswordPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/recovery-codes\n  method: post\n  operationId: GenerateUserRecoveryCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/recovery-codes/signin\n\
  \  method: post\n  operationId: SignInRecoveryCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/saml/authorize\n  method: post\n  operationId: CreateSAMLRedirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/saml/exchange\n  method: post\n  operationId: ExchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/auth/saml/idp/metadata\n  method: get\n  operationId: SAMLIDPMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/security-questions/setup\n  method: post\n  operationId: SetupUserSecurityQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/security-questions/verify\n  method: get\n  operationId: GetUserSecurityVerifyQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/security-questions/verify\n  method: post\n  operationId: VerifyUserSecurityQuestions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/sso/authorize\n  method: post\n  operationId: AuthorizeSAML\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/sso/exchange\n  method: post\n  operationId: ExchangeCodesso\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/totp/signup\n\
  \  method: post\n  operationId: SignUpTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/totp/verify\n  method: post\n  operationId: VerifyCodeTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/totp/update\n  method: post\n  operationId: UpdateUserTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auth/webauthn/signup/start\n  method: post\n  operationId: WebAuthnSignupStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/signup/finish\n  method: post\n  operationId: WebAuthnSignupFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/signin/start\n  method: post\n  operationId: WebAuthnSigninStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/signin/finish\n  method: post\n  operationId: WebAuthnSigninFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/signup-in/start\n  method: post\n  operationId: WebAuthnSignUpInStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/update/start\n  method: post\n  operationId: WebAuthnDeviceAddStart\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/webauthn/update/finish\n  method: post\n  operationId: WebAuthnDeviceAddFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/wsfed/idp/metadata\n  method: get\n  operationId: WSFedIDPMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mgmt/user/customattributes\n  method: get\n  operationId: UserCustomAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mgmt/user/customattribute/create\n  method: post\n  operationId: CreateUserCustomAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mgmt/user/customattribute/delete\n  method: post\n  operationId: DeleteUserCustomAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/signup/email\n  method: post\n  operationId: SignUpEnchantedLink\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/signin/email\n  method: post\n  operationId: SignInEnchantedLinkEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/signup-in/email\n  method: post\n  operationId: SignUpOrInEnchantedLinkEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/verify\n\
  \  method: post\n  operationId: VerifyEnchantedLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/pending-session\n  method: post\n  operationId: GetEnchantedLinkSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/enchantedlink/update/email\n  method: post\n  operationId: UpdateUserEmailEnchantedLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/notp/{provider}/signup\n  method: post\n  operationId: SignUpNOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/notp/{provider}/signin\n  method: post\n  operationId: SignInNOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/notp/{provider}/signup-in\n  method: post\n  operationId: SignUpOrInNOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/notp/pending-session\n  method: post\n  operationId: GetNOTPSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/magiclink/signup/email\n  method: post\n  operationId: SignUpMagicLinkEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/magiclink/signin/email\n  method: post\n  operationId: SignInMagicLinkEmail\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/magiclink/signup-in/email\n  method: post\n  operationId: SignUpOrInMagicLinkEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/magiclink/update/email\n  method: post\n  operationId: UpdateUserEmailMagicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auth/otp/signup/email\n  method: post\n  operationId: UserSignupOtpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/signin/email\n  method: post\n  operationId: UserSigninOtpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/signup-in/email\n  method: post\n  operationId: UserSignUpInOtpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/verify/email\n  method: post\n  operationId: VerifyOtpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/update/email\n  method: post\n  operationId: UpdateUserEmailOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/password/reset\n  method: post\n  operationId: SendPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/mgmt/user/signin/embeddedlink\n  method: post\n  operationId: EmbeddedLinkSignin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fedcm/clientmetadata\n  method: get\n  operationId: GetFedCMClientMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{projectId}/fedcm/config\n  method: get\n  operationId: GetFedCMConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/otp/signup/im\n  method: post\n  operationId: SignUpOTPInstantMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/signin/im\n  method: post\n  operationId: SignInOTPInstantMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/signup-in/im\n  method: post\n  operationId: SignUpOrInOTPInstantMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/verify/im\n  method: post\n  operationId: VerifyCodeIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp/update/phone/im\n  method: post\n  operationId: UpdateUserPhoneOTPIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{projectId}\n  method: get\n  operationId: GetKeys\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/keys/{projectId}\n  method: get\n  operationId: GetKeysV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mgmt/inboundapp/app/{projectId}/register\n  method: post\n  operationId: RegisterThirdPartyApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (146 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/agentic-access/descope-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/agentic-access/descope-agentic-access.yml
summary_line: 459 operations · 350 acting · 8 human-in-the-loop
tags:
- Authentication
- Identity
- CIAM
- Passwordless
- Passkeys
- MFA
- SSO
- OIDC
- SAML
- SCIM
- Authorization
- FGA
- Agentic Identity
- MCP
- Identity Federation
---
