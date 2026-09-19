---
acting_count: 71
action_class_counts:
  acting: 71
  connected: 40
api_specs:
- filename: authelia-authentication-api-openapi.yml
  format: yaml
  label: Authelia Authentication API
  slug: authelia-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authentication-api-openapi.yml
- filename: authelia-authorization-api-openapi.yml
  format: yaml
  label: Authelia Authorization API
  slug: authelia-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authorization-api-openapi.yml
- filename: authelia-first-factor-api-openapi.yml
  format: yaml
  label: Authelia First Factor API
  slug: authelia-first-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-first-factor-api-openapi.yml
- filename: authelia-oauth-2-0-api-openapi.yml
  format: yaml
  label: Authelia OAuth 2.0 API
  slug: authelia-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-oauth-2-0-api-openapi.yml
- filename: authelia-openid-connect-1-0-api-openapi.yml
  format: yaml
  label: Authelia OpenID Connect 1.0 API
  slug: authelia-openid-connect-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-openid-connect-1-0-api-openapi.yml
- filename: authelia-password-change-api-openapi.yml
  format: yaml
  label: Authelia Password Change API
  slug: authelia-password-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-change-api-openapi.yml
- filename: authelia-password-reset-api-openapi.yml
  format: yaml
  label: Authelia Password Reset API
  slug: authelia-password-reset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-reset-api-openapi.yml
- filename: authelia-second-factor-api-openapi.yml
  format: yaml
  label: Authelia Second Factor API
  slug: authelia-second-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-second-factor-api-openapi.yml
- filename: authelia-state-api-openapi.yml
  format: yaml
  label: Authelia State API
  slug: authelia-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-state-api-openapi.yml
- filename: authelia-user-elevation-api-openapi.yml
  format: yaml
  label: Authelia User Elevation API
  slug: authelia-user-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-elevation-api-openapi.yml
- filename: authelia-user-information-api-openapi.yml
  format: yaml
  label: Authelia User Information API
  slug: authelia-user-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-information-api-openapi.yml
- filename: authelia-utilities-api-openapi.yml
  format: yaml
  label: Authelia Utilities API
  slug: authelia-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-utilities-api-openapi.yml
consequence_counts:
  read: 40
  safety-critical: 11
  write: 60
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Authelia Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/authorization
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/authorization
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/consent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/consent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/oidc/userinfo
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/reset-password/identity/finish
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/reset-password/identity/start
operation_count: 111
overview: 'Authelia exposes 111 API operations that an AI agent could call, of which 71 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 60 write, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Authelia
provider_slug: authelia
slug: authelia-agentic-access
source_filename: authelia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/authelia-authentication-api-openapi.yml, openapi/authelia-authorization-api-openapi.yml,\n  openapi/authelia-first-factor-api-openapi.yml, openapi/authelia-oauth-2-0-api-openapi.yml,\n  openapi/authelia-openid-connect-1-0-api-openapi.yml, openapi/authelia-password-change-api-openapi.yml,\n  openapi/authelia-password-reset-api-openapi.yml, openapi/authelia-second-factor-api-openapi.yml,\n  openapi/authelia-state-api-openapi.yml, openapi/authelia-user-elevation-api-openapi.yml, openapi/authelia-user-information-api-openapi.yml,\n  openapi/authelia-utilities-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 111\n  by_action_class:\n    acting: 71\n    connected: 40\n  by_consequence:\n\
  \    write: 60\n    read: 40\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /api/firstfactor\n  method: post\n  operationId: postFirstFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/firstfactor/reauthenticate\n  method: post\n  operationId: postFirstFactorReauthenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/firstfactor/passkey\n  method: get\n  operationId: getFirstFactorPasskey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/firstfactor/passkey\n  method: post\n  operationId: postFirstFactorPasskey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/logout\n  method: post\n  operationId: postLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: get\n  operationId: getSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/secondfactor/totp/register\n  method: put\n  operationId: putSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: post\n  operationId: postSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: delete\n  operationId: deleteSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp\n  method: get\n  operationId: getSecondFactorTOTPConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/totp\n  method: post\n  operationId: postSecondFactorTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp\n  method: delete\n  operationId: deleteSecondFactorTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn\n  method: get\n  operationId: getSecondFactorWebAuthn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/webauthn\n  method: post\n  operationId: postSecondFactorWebAuthn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credentials\n  method: get\n  operationId: getSecondFactorWebAuthnCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/secondfactor/webauthn/credential/register\n  method: put\n  operationId: putSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/register\n  method: post\n  operationId: postSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/register\n  method: delete\n  operationId: deleteSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/{credentialID}\n  method: put\n  operationId: putSecondFactorWebAuthnCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/{credentialID}\n  method: delete\n  operationId: deleteSecondFactorWebAuthnCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/duo\n  method: get\n  operationId: getSecondFactorDuo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/duo\n  method: post\n  operationId: postSecondFactorDuo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/duo_devices\n  method: get\n  operationId: getSecondFactorDuoDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/duo_device\n  method: post\n  operationId: postSecondFactorDuoDevice\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/password\n  method: post\n  operationId: postSecondFactorPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/authz/auth-request\n  method: get\n  operationId: getAuthzAuthRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/auth-request\n  method: head\n  operationId: headAuthzAuthRequest\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/ext-authz\n  method: get\n  operationId: getAuthzExtAuthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/ext-authz\n  method: head\n  operationId: headAuthzExtAuthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/ext-authz\n  method: options\n  operationId: optionsAuthzExtAuthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/ext-authz\n  method: post\n  operationId: postAuthzExtAuthz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/authz/ext-authz\n  method: put\n  operationId: putAuthzExtAuthz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/authz/ext-authz\n  method: patch\n  operationId: patchAuthzExtAuthz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/authz/ext-authz\n  method: delete\n  operationId: deleteAuthzExtAuthz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/authz/forward-auth\n  method: get\n  operationId: getAuthzForwardAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authz/forward-auth\n  method: head\n  operationId: headAuthzForwardAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify\n  method: get\n  operationId: getAuthzLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify\n  method: head\n  operationId: headAuthzLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify\n  method: options\n  operationId: optionsAuthzLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify\n  method: post\n  operationId: postAuthzLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify\n  method: put\n  operationId: putAuthzLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify\n\
  \  method: patch\n  operationId: patchAuthzLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify\n  method: delete\n  operationId: deleteAuthzLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/firstfactor\n  method: post\n  operationId: postFirstFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/firstfactor/reauthenticate\n  method: post\n  operationId: postFirstFactorReauthenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/firstfactor/passkey\n  method: get\n  operationId: getFirstFactorPasskey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/firstfactor/passkey\n  method: post\n  operationId: postFirstFactorPasskey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuth2AuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jwks.json\n  method: get\n  operationId: getOpenIDConnectJSONWebKeySet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/authorization\n  method: get\n  operationId: getOpenIDConnectAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/authorization\n  method: post\n  operationId: postOpenIDConnectAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/oidc/device-authorization\n  method: post\n  operationId: postOAuth2DeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/device-authorization\n  method: put\n  operationId: putOAuth2DeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/pushed-authorization-request\n  method: post\n  operationId: postOAuth2PushedAuthorizationRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/token\n  method: post\n  operationId: postOpenIDConnectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/oidc/revocation\n  method: post\n  operationId: postOAuth2Revocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/oidc/introspection\n  method: post\n  operationId: postOAuth2Introspection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/consent\n  method: get\n  operationId: getOpenIDConnectConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/consent\n  method: post\n  operationId: postOpenIDConnectConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: getOpenIDConnectConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jwks.json\n  method: get\n  operationId: getOpenIDConnectJSONWebKeySet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/authorization\n  method: get\n  operationId: getOpenIDConnectAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/authorization\n  method: post\n  operationId: postOpenIDConnectAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/oidc/device-authorization\n  method: post\n  operationId: postOAuth2DeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/device-authorization\n  method: put\n  operationId: putOAuth2DeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/pushed-authorization-request\n  method: post\n  operationId: postOAuth2PushedAuthorizationRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/token\n  method: post\n  operationId: postOpenIDConnectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/oidc/revocation\n  method: post\n  operationId: postOAuth2Revocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/oidc/introspection\n  method: post\n  operationId: postOAuth2Introspection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oidc/userinfo\n  method: get\n  operationId: getOpenIDConnectUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/userinfo\n  method: post\n  operationId: postOpenIDConnectUserInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n  \
  \  audit: required\n- path: /api/oidc/consent\n  method: get\n  operationId: getOpenIDConnectConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oidc/consent\n  method: post\n  operationId: postOpenIDConnectConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/change-password\n  method: post\n  operationId: postChangePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/reset-password/identity/start\n  method: post\n  operationId: postResetPasswordIdentityStart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/reset-password/identity/finish\n  method: post\n  operationId: postResetPasswordIdentityFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/reset-password\n  method: post\n  operationId: postResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/reset-password\n  method: delete\n  operationId: deleteResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: get\n  operationId: getSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/totp/register\n  method: put\n  operationId: putSecondFactorTOTPRegistration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: post\n  operationId: postSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp/register\n  method: delete\n  operationId: deleteSecondFactorTOTPRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/secondfactor/totp\n  method: get\n  operationId: getSecondFactorTOTPConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/totp\n  method: post\n  operationId: postSecondFactorTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/totp\n  method: delete\n  operationId: deleteSecondFactorTOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/secondfactor/webauthn\n  method: get\n  operationId: getSecondFactorWebAuthn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/webauthn\n  method: post\n  operationId: postSecondFactorWebAuthn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credentials\n  method: get\n  operationId: getSecondFactorWebAuthnCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/webauthn/credential/register\n  method: put\n  operationId: putSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/register\n  method: post\n  operationId: postSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/register\n  method: delete\n  operationId: deleteSecondFactorWebAuthnCredentialRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/{credentialID}\n  method: put\n  operationId: putSecondFactorWebAuthnCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/webauthn/credential/{credentialID}\n  method: delete\n  operationId: deleteSecondFactorWebAuthnCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/duo\n  method: get\n  operationId: getSecondFactorDuo\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/duo\n  method: post\n  operationId: postSecondFactorDuo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/duo_devices\n  method: get\n  operationId: getSecondFactorDuoDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/secondfactor/duo_device\n  method: post\n  operationId: postSecondFactorDuoDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/secondfactor/password\n  method: post\n  operationId: postSecondFactorPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/configuration\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/configuration/password-policy\n  method: get\n  operationId: getPasswordPolicyConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: head\n  operationId: headHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequ\n\n# --- truncated at 32 KB (34 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/agentic-access/authelia-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/agentic-access/authelia-agentic-access.yml
summary_line: 111 operations · 71 acting · 11 human-in-the-loop
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open-Source
- OpenID Connect
- Self-Hosted
- SSO
---
