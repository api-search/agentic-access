---
acting_count: 272
action_class_counts:
  acting: 272
  connected: 186
api_specs:
- filename: auth0-management-api-openapi.yml
  format: yaml
  label: Auth0 Management API
  slug: auth0-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-management-api-openapi.yml
- filename: auth0-authentication-api-openapi.yml
  format: yaml
  label: Auth0 Authentication API
  slug: auth0-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-authentication-api-openapi.yml
- filename: auth0-fga-openapi.yml
  format: yaml
  label: Auth0 FGA (Fine-Grained Authorization)
  slug: auth0-fga
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-fga-openapi.yml
consequence_counts:
  physical: 20
  read: 186
  safety-critical: 11
  write: 241
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Auth0 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /branding/phone/templates/{id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /keys/signing/{kid}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /network-acls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /network-acls/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /network-acls/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /network-acls/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /refresh-tokens/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /self-service-profiles/{profileId}/sso-ticket/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sessions/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/{id}/revoke-access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /actions/actions/{actionId}/versions/{id}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /actions/actions/{id}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /branding/phone/providers/{id}/try
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /branding/phone/templates/{id}/try
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /connections/{id}/directory-provisioning
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /connections/{id}/directory-provisioning
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connections/{id}/directory-provisioning
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connections/{id}/directory-provisioning/synchronizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /connections/{id}/directory-provisioning/synchronized-groups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /dbconnections/change_password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /event-streams/{id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /jobs/verification-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stores/{store_id}/batch-check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stores/{store_id}/check
operation_count: 458
overview: 'Auth0 exposes 458 API operations that an AI agent could call, of which 272 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 186 read, 241 write, 20 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Auth0
provider_slug: auth0
slug: auth0-agentic-access
source_filename: auth0-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/auth0-authentication-api-openapi.yml, openapi/auth0-fga-openapi.yml, openapi/auth0-management-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 458\n  by_action_class:\n    connected: 186\n    acting: 272\n  by_consequence:\n    read: 186\n    write: 241\n    physical: 20\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/logout\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oidc/logout\n  method: get\n  operationId: oidc_logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /samlp/{CLIENT_ID}/logout\n  method: post\n  operationId: saml_logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passwordless/start\n  method: post\n  operationId: passwordless_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /passwordless/verify\n  method: post\n  operationId: passwordless_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: oauth_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbconnections/signup\n  method: post\n  operationId: dbconnections_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /dbconnections/change_password\n  method: post\n  operationId: dbconnections_change_password\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userinfo\n  method: get\n  operationId: userinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mfa/challenge\n  method: post\n  operationId: mfa_challenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /mfa/associate\n  method: post\n  operationId: mfa_associate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mfa/authenticators\n  method: get\n  operationId: mfa_authenticators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mfa/authenticators/{AUTHENTICATOR_ID}\n  method: delete\n  operationId: mfa_authenticators_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /samlp/{client_id}\n  method: get\n  operationId: samlp_login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /samlp/metadata/{client_id}\n  method: get\n  operationId: samlp_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login/callback\n  method: post\n  operationId: login_callback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wsfed/{client_id}\n  method: get\n  operationId: wsfed_login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /wsfed/FederationMetadata/2007-06/FederationMetadata.xml\n  method: get\n  operationId: wsfed_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oidc/register\n  method: post\n  operationId: oidc_register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/device/code\n  method: post\n  operationId: oauth_device_code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/revoke\n  method:\
  \ post\n  operationId: oauth_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/access_token\n  method: post\n  operationId: oauth_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/ro\n  method: post\n  operationId: oauth_ro\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /tokeninfo\n  method: post\n  operationId: tokeninfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delegation\n  method: post\n  operationId: delegation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unlink\n  method: post\n  operationId: unlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/impersonate\n  method: post\n  operationId: impersonate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/authzen-configuration/{store_id}\n  method: get\n  operationId: GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores\n  method: get\n  operationId: ListStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores\n  method: post\n  operationId: CreateStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}\n  method: get\n  operationId: GetStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_id}\n  method: delete\n  operationId: DeleteStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/access/v1/evaluation\n  method: post\n  operationId: Evaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/access/v1/evaluations\n  method: post\n  operationId: Evaluations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/access/v1/search/action\n  method: post\n  operationId: ActionSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/access/v1/search/resource\n  method: post\n  operationId: ResourceSearch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/access/v1/search/subject\n  method: post\n  operationId: SubjectSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/assertions/{authorization_model_id}\n  method: get\n  operationId: ReadAssertions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_id}/assertions/{authorization_model_id}\n  method: put\n  operationId: WriteAssertions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/authorization-models\n  method: get\n  operationId: ReadAuthorizationModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_id}/authorization-models\n  method: post\n  operationId: WriteAuthorizationModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/authorization-models/{id}\n  method: get\n  operationId: ReadAuthorizationModel\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_id}/batch-check\n  method: post\n  operationId: BatchCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/changes\n  method: get\n  operationId: ReadChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_id}/check\n  method: post\n  operationId: Check\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/expand\n  method: post\n  operationId: Expand\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/list-objects\n  method: post\n  operationId: ListObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /stores/{store_id}/list-users\n  method: post\n  operationId: ListUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/read\n  method: post\n  operationId: Read\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/streamed-list-objects\n  method: post\n  operationId: StreamedListObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_id}/write\n  method: post\n  operationId: Write\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions\n  method: get\n  operationId: get_actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/actions\n  method: post\n  operationId: post_action\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions/{actionId}/versions\n  method: get\n  operationId: get_action_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/actions/{actionId}/versions/{id}\n  method: get\n  operationId: get_action_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/actions/{actionId}/versions/{id}/deploy\n  method: post\n  operationId: post_deploy_draft_version\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:actions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions/{id}\n  method: get\n  operationId: get_action\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/actions/{id}\n  method: delete\n  operationId: delete_action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions/{id}\n\
  \  method: patch\n  operationId: patch_action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions/{id}/deploy\n  method: post\n  operationId: post_deploy_action\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:actions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/actions/{id}/test\n  method: post\n  operationId: post_test_action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - create:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/executions/{id}\n  method: get\n  operationId: get_execution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/modules\n  method: get\n  operationId: get_action_modules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/modules\n  method: post\n  operationId: post_action_module\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/modules/{id}\n  method: get\n  operationId: get_action_module\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/modules/{id}\n  method: delete\n  operationId: delete_action_module\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/modules/{id}\n  method: patch\n  operationId: patch_action_module\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:actions\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/modules/{id}/actions\n  method: get\n  operationId: get_action_module_actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/modules/{id}/rollback\n  method: post\n  operationId: post_action_module_rollback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/modules/{id}/versions\n  method: get\n  operationId: get_action_module_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/modules/{id}/versions\n  method: post\n  operationId: post_action_module_version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/modules/{id}/versions/{versionId}\n  method: get\n  operationId: get_action_module_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/triggers\n  method: get\n  operationId: get_triggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /actions/triggers/{triggerId}/bindings\n  method: get\n  operationId: get_bindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:actions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/triggers/{triggerId}/bindings\n  method: patch\n  operationId: patch_bindings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:actions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /anomaly/blocks/ips/{id}\n  method: get\n  operationId: get_ips_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:anomaly_blocks\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /anomaly/blocks/ips/{id}\n\
  \  method: delete\n  operationId: delete_ips_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:anomaly_blocks\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attack-protection/bot-detection\n  method: get\n  operationId: get_bot-detection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:attack_protection\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack-protection/bot-detection\n  method: patch\n  operationId: patch_bot-detection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:attack_protection\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /attack-protection/breached-password-detection\n  method: get\n  operationId: get_breached-password-detection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:attack_protection\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack-protection/breached-password-detection\n  method: patch\n  operationId: patch_breached-password-detection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:attack_protection\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attack-protection/brute-force-protection\n  method: get\n  operationId: get_brute-force-protection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read:attack_protection\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack-protection/brute-force-protection\n  method: patch\n  operationId: patch_brute-force-protection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:attack_protection\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attack-protection/captcha\n  method: get\n  operationId: get_captcha\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:attack_protection\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack-protection/captcha\n  method: patch\n  operationId: patch_captcha\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ update:attack_protection\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attack-protection/suspicious-ip-throttling\n  method: get\n  operationId: get_suspicious-ip-throttling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:attack_protection\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack-protection/suspicious-ip-throttling\n  method: patch\n  operationId: patch_suspicious-ip-throttling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:attack_protection\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding\n  method: get\n  operationId: get_branding\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:branding\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branding\n  method: patch\n  operationId: patch_branding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:branding\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/providers\n  method: get\n  operationId: get_branding_phone_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:phone_providers\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branding/phone/providers\n  method: post\n  operationId: create_phone_provider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - create:phone_providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/providers/{id}\n  method: get\n  operationId: get_phone_provider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:phone_providers\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branding/phone/providers/{id}\n  method: delete\n  operationId: delete_phone_provider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:phone_providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/providers/{id}\n  method: patch\n  operationId:\
  \ update_phone_provider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - update:phone_providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/providers/{id}/try\n  method: post\n  operationId: try_phone_provider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:phone_providers\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/templates\n  method: get\n  operationId: get_phone_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - read:phone_templates\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branding/phone/templates\n  method: post\n  operationId: create_phone_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:phone_templates\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/phone/templates/{id}\n  method: get\n  operationId: get_phone_template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:phone_templates\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branding/phone/templates/{id}\n  method: delete\n  operationId: delete_phone_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:phone_templates\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: \n\n# --- truncated at 32 KB (152 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/agentic-access/auth0-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/agentic-access/auth0-agentic-access.yml
summary_line: 458 operations · 272 acting · 11 human-in-the-loop
tags:
- AI Agents
- Authentication
- Authorization
- FGA
- Identity Management
- MCP
- OAuth
- Okta
- OpenID Connect
- SAML
- Security
- SCIM
---
