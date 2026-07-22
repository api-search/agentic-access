---
acting_count: 419
action_class_counts:
  acting: 419
  connected: 303
api_specs:
- filename: socotra-openapi-original.json
  format: json
  label: Socotra Insurance Suite API
  slug: socotra-insurance-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-openapi-original.json
consequence_counts:
  physical: 39
  read: 303
  safety-critical: 12
  write: 368
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Socotra Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /auth/users/{locator}/passwordreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/users/{locator}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /billing/{tenantLocator}/creditDistributions/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /billing/{tenantLocator}/disbursements/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /billing/{tenantLocator}/holds/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /billing/{tenantLocator}/payments/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /claim/{tenantLocator}/fnols/{fnolLocator}/losses/{lossLocator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /policy/{tenantLocator}/deserializeJobs/{locator}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /policy/{tenantLocator}/quickquotes/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /policy/{tenantLocator}/quotes/{locator}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /policy/{tenantLocator}/transactions/{locator}/elements
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /policy/{tenantLocator}/transactions/{locator}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/accounts/{accountLocator}/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/accounts/{accountLocator}/charges/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices/earlyInvoicing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /billing/{tenantLocator}/invoices/{locator}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /billing/{tenantLocator}/invoices/{locator}/aggregated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices/{locator}/number/generate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices/{locator}/number/set
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices/{locator}/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/invoices/{locator}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /billing/{tenantLocator}/invoices/{locator}/writeOff
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/{tenantLocator}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /billing/{tenantLocator}/payments/{locator}
operation_count: 722
overview: 'Socotra exposes 722 API operations that an AI agent could call, of which 419 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 303 read, 368 write, 39 physical, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Socotra
provider_slug: socotra
slug: socotra-agentic-access
source_filename: socotra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/socotra-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 722\n  by_action_class:\n    connected: 303\n    acting: 419\n  by_consequence:\n    read: 303\n    write: 368\n    safety-critical: 12\n    physical: 39\n  human_in_the_loop_required: 12\noperations:\n- path: /auth/identity/passwordPolicy\n  method: get\n  operationId: fetchPasswordPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/identity/passwordPolicy\n  method: put\n  operationId: updatePasswordPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/tokens\n  method: get\n  operationId: fetchAuthTokensForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/tokens\n  method: post\n  operationId: createServiceAccountAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/revoke\n  method: post\n  operationId: revokeUserOauthTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/users/tokens\n  method: get\n  operationId: fetchAuthTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/tokens\n  method: post\n  operationId: createAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/tokens/permissions\n  method: post\n  operationId: getGroupedTokenPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles/tenant/{tenantLocator}/{roleLocator}\n  method: get\n  operationId: getTenantRole\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/roles/tenant/{tenantLocator}/{roleLocator}\n  method: post\n  operationId: createTenantRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles/tenant/{tenantLocator}/{roleLocator}\n  method: patch\n  operationId: updateTenantRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles/tenant/{tenantLocator}/{roleLocator}\n  method: delete\n  operationId: deleteTenantRole\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/identity\n  method: post\n  operationId: createIdentityProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/identity/saml\n  method: post\n  operationId: addSAMLIdentityProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/identity/oidc\n\
  \  method: post\n  operationId: addOIDCIdentityProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}\n  method: get\n  operationId: fetchUserByLocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/tenants\n  method: patch\n  operationId: updateUserTenantAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/roles\n  method: patch\n  operationId: updateUserRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /auth/users/{locator}/passwordreset\n  method: patch\n  operationId: resetUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/users/{locator}/enable\n  method: patch\n  operationId: enableUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/dataaccess/{tenantLocator}\n  method: get\n  operationId: fetchUserDataAccessForTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /auth/users/{locator}/dataaccess/{tenantLocator}\n  method: patch\n  operationId: addUserDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/dataaccess/{tenantLocator}\n  method: delete\n  operationId: deleteUserDataAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/accessmask\n  method: get\n  operationId: fetchUserMasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/accessmask\n  method: patch\n  operationId: addDataSecurityMask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/tenants/{locator}\n  method: get\n  operationId: fetchTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/tenants/{locator}\n  method: patch\n  operationId: updateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/tenants/{locator}/retire\n\
  \  method: patch\n  operationId: retireTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles/{locator}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/roles/{locator}\n  method: patch\n  operationId: updateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/roles/{locator}\n  method: delete\n  operationId: deleteRole\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{userLocator}/tenant/{tenantLocator}/permissions\n  method: get\n  operationId: fetchUserTenantPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/permissions\n  method: get\n  operationId: fetchUserPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/dataaccess\n  method: get\n  operationId: fetchUserDataAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /auth/users/{locator}/credentialStatus\n  method: get\n  operationId: fetchCredentialStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/accessmask/{tenantLocator}\n  method: get\n  operationId: fetchUserMasksForTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/{locator}/accessmask/{tenantLocator}\n  method: delete\n  operationId: deleteUserMasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/accessmask/{tenantLocator}/{type}\n  method: get\n  operationId: fetchUserMask\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/whoami\n  method: get\n  operationId: fetchMyUserDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/username/{username}\n  method: get\n  operationId: fetchUserByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/list\n  method: get\n  operationId: fetchMultipleUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/users/basic/list\n  method: get\n  operationId: fetchMultipleBasicUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /auth/tenants/mytenants/list\n  method: get\n  operationId: fetchMyTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/tenants/list\n  method: get\n  operationId: fetchTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/roles/tenant/{tenantLocator}/list\n  method: get\n  operationId: listTenantRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/roles/permissions\n  method: get\n  operationId: fetchAvailablePermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/roles/list\n  method:\
  \ get\n  operationId: fetchMultipleRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/identity/instances\n  method: get\n  operationId: fetchIdentityProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/identity/instances/{name}\n  method: get\n  operationId: fetchIdentityProviderByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/identity/instances/{name}\n  method: delete\n  operationId: deleteIdentityServerInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /auth/users/{locator}/tokens/{tokenOrName}\n  method: delete\n  operationId: deleteAuthTokenForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{locator}/credentials\n  method: delete\n  operationId: removeCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/tokens/{tokenOrName}\n  method: delete\n  operationId: deleteAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/auxdata/{locator}\n  method: get\n  operationId: getAuxDataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/auxdata/{locator}\n  method: put\n  operationId: putAuxData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/mediadata\n  method: post\n  operationId: createMediaData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/diary/{referenceType}/{referenceLocator}\n  method: get\n  operationId: fetchLatestDiaryEntriesByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/diary/{referenceType}/{referenceLocator}\n  method: post\n  operationId: createDiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/diary/segments/{segmentLocator}/element/{staticElementLocator}\n  method: post\n  operationId: createDiaryForSegmentElement\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/diary/quotes/{quoteLocator}/element/{staticElementLocator}\n  method: post\n  operationId: createDiaryForQuoteElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/mediadata/{locator}\n  method: get\n  operationId: fetchLatestMediaData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/mediadata/{locator}\n  method:\
  \ patch\n  operationId: updateMediaData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/mediadata/{locator}\n  method: delete\n  operationId: deleteMediaData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/diary/{locator}\n  method: get\n  operationId: fetchAllDiaryEntriesByLocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/diary/{locator}\n\
  \  method: patch\n  operationId: updateDiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/diary/{locator}/discard\n  method: patch\n  operationId: discardDiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/mediadata/{locator}/versions/{versionLocator}\n  method: get\n  operationId: fetchMediaData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/mediadata/{locator}/versions/{versionLocator}/file\n\
  \  method: get\n  operationId: fetchFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/mediadata/{locator}/list\n  method: get\n  operationId: fetchAllMediaDataByLocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/mediadata/{locator}/file\n  method: get\n  operationId: fetchLatestFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/mediadata/search/{referenceType}/{referenceLocator}/list\n  method: get\n  operationId: fetchLatestMediaDataByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /auxdata/{tenantLocator}/diary/{locator}/latest\n  method: get\n  operationId: fetchLatestDiaryEntryByLocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/auxdata/{locator}/{key}\n  method: get\n  operationId: getAuxData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auxdata/{tenantLocator}/auxdata/{locator}/{key}\n  method: delete\n  operationId: deleteAuxData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auxdata/{tenantLocator}/auxdata/size\n  method: get\n  operationId: getAuxDataSize\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/{tenantLocator}/payments/{locator}\n  method: get\n  operationId: fetchPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/{tenantLocator}/payments/{locator}\n  method: put\n  operationId: updatePaymentOverwriteData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/payments/{locator}\n  method: patch\n  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/disbursements/{locator}\n  method: get\n  operationId: fetchDisbursement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/{tenantLocator}/disbursements/{locator}\n  method: put\n  operationId: updateDisbursementReplaceData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/disbursements/{locator}\n  method: patch\n  operationId: updateDisbursement\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/creditDistributions/{locator}\n  method: get\n  operationId: fetchCreditDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/{tenantLocator}/creditDistributions/{locator}\n  method: put\n  operationId: createOrReplaceCreditDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/creditDistributions/{locator}\n  method:\
  \ patch\n  operationId: updateCreditDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/writeOffs\n  method: post\n  operationId: writeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/retryJobs/{policyLocator}/retryFailedTransactions\n  method: post\n  operationId: retryFailedTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/payments/{locator}/number/set\n  method: post\n  operationId: setPaymentNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/payments/{locator}/number/generate\n\
  \  method: post\n  operationId: generatePaymentNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/jobs/delinquencies/moratoriums\n  method: post\n  operationId: runDelinquencyMoratoriumsWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices\n  method: post\n  operationId: createAggregatedInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices/{locator}/transfer\n  method: post\n  operationId: transferInvoicesBetweenAggregatedInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices/{locator}/settle\n  method: post\n  operationId: settleNegativeOrZeroInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices/{locator}/number/set\n  method: post\n  operationId: setInvoiceNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices/{locator}/number/generate\n  method: post\n  operationId: generateInvoiceNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /billing/{tenantLocator}/invoices/earlyInvoicing\n  method: post\n  operationId: initiateEarlyInvoicing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/holds\n  method: post\n  operationId: createHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/{tenantLocator}/financialInstruments\n  method: post\n  operationId: createFinancialInstrument\n  x-agentic-acc\n\n# --- truncated at 32\
  \ KB (232 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/agentic-access/socotra-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/agentic-access/socotra-agentic-access.yml
summary_line: 722 operations · 419 acting · 12 human-in-the-loop
tags:
- Company
- Insurtech
- Insurance
- Core Platform
- Policy Administration
- Billing
- Claims
- Underwriting
- API
- MCP
---
